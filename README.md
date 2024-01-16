# [ZeroTier Pylon](https://github.com/zerotier/pylon) собранный статически
С помощью [gost](https://github.com/go-gost/gost), например,  можно пробросить порт<br />
  на сервере:<br />
  `pylon refract <net_id> --listen-addr 0.0.0.0 --listen-port 1111`
  
  в клиенте:<br />
  `gost -L='tcp://127.0.0.1:8080/127.0.0.1:80' -F='socks5://<ваша сеть>:1111'`
<br /><br />
И не забывайте - `While a single Pylon instance will work for multiple networks and multiple applications simultaneously it will perform better if a new instance is started for each proxied network. The underlying libzt isn't multithreaded so it is recommended that you also split your proxied traffic across multiple instances if you notice performance bottlecks.` 


Со своей стороны рекомендую присмотреться к [yggstack](https://github.com/yggdrasil-network/yggstack)
<br /><br /><br />
 * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
 * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
 * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
 * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 * POSSIBILITY OF SUCH DAMAGE.
 
