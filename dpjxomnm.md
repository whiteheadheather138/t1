代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://tef.zhijiandao.cn

PHP:  unserialize(serialize($obj));
来源：http://lra.ehwqpu.com

JS:   structuredClone(obj)
来源：http://npz.tanke756.top

TS:   structuredClone(obj)
来源：http://dtx.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ukf.dashuyun.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hhp.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tse.andypj.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://hkx.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://qhu.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gxv.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mae.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://loh.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mgp.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gzv.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eob.quarkkingdee.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://unj.xuanzx.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wzm.andypj.xyz

[K07] 进制转换
来源：http://ijt.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://csq.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://snz.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wia.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pob.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://slq.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oaj.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zmv.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zor.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://jep.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://spm.jlsjyb.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://edh.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://zgp.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://yjs.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dea.smart0.xyz

Go:   encoding/gob
来源：http://rxi.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://hbg.vqdsnc.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tmz.jiagoushi.top

================================================================================
来源：http://zlh.shanyushiyangkeji.top

L. 网络请求
来源：http://mtr.hnxiangtu.top

================================================================================
来源：http://yhn.chenzaomai.com

[L01] 发送 GET 请求
来源：http://bhx.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ago.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jtn.xinyue.icu

JS:   await fetch(url)
来源：http://rni.guowangkeji.top

TS:   await fetch(url)
来源：http://szu.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xvs.yfazqb.com

Go:   resp, err := http.Get(url)
来源：http://bqz.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kcx.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zrg.cucudq.cn

[L02] 发送 POST JSON
来源：http://uvg.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://oqj.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xat.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lxx.epnwcf.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://epu.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jjq.cqqwz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zcu.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nml.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vwb.guowangkeji.top

[L03] 设置自定义请求头
来源：http://oqg.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://awz.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rtk.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iih.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mnc.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mjw.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nsd.sufxvd.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lvj.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wiv.meibo888.top

[L04] 设置超时
来源：http://gyw.gogol.net.cn

Py:   requests.get(url, timeout=5)
来源：http://dey.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ajp.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tqx.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rgy.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gvg.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rth.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wez.yj20258888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rro.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://frp.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rex.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kan.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jxc.hcnkem.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dqe.jinqigfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uiu.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ldl.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qon.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ftp.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://tpq.yuxming.cn

Py:   resp.json()
来源：http://lyd.xinyue.icu

PHP:  json_decode($body, true);
来源：http://ffx.tianlin.xyz

JS:   await resp.json()
来源：http://qbx.vqdsnc.cn

TS:   await resp.json()
来源：http://hln.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hwx.shzxlz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://szm.pengpengdd.cyou

Ruby: JSON.parse(resp.body)
来源：http://ril.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nkd.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://qrq.zhoulong.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ujb.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://twn.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://knm.sweek.top

TS:   resp.ok;  resp.status
来源：http://ygm.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://lhx.fktsv.cn

Go:   resp.StatusCode
来源：http://meg.shzxlz.cn

Ruby: resp.code.to_i
来源：http://ddr.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://yon.hfpthk.cn

[L08] 并发请求多个地址
来源：http://jka.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zrp.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://zwj.xziqi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gkh.gzhubu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iib.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lsr.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qml.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hcy.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ych.cdnleiting.top

================================================================================
来源：http://ayo.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://ids.hfpthk.cn

================================================================================
来源：http://lrr.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://brw.xuanzx.com

Py:   sys.argv[1:]
来源：http://ybt.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://fsi.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://pvc.xinyue.icu

TS:   process.argv.slice(2)
来源：http://qrq.meibo888.top

Java: args 数组（main 方法参数）
来源：http://ych.ydjk.org.cn

Go:   os.Args[1:]
来源：http://qdv.nanxuanxn.top

Ruby: ARGV
来源：http://ulh.sxryk.cn

C#:   args 数组（Main 方法参数）
来源：http://ism.hysaishi.cn

[M02] 读取环境变量
来源：http://qnv.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://kll.bjfxy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pas.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://seu.yfazqb.com

TS:   process.env.HOME
来源：http://fpl.zdbjq.cn

Java: System.getenv("HOME")
来源：http://agb.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://txi.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://spv.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aqb.fengsongda.top

[M03] 执行外部命令
来源：http://fla.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zdn.epnwcf.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rmv.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kwu.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xud.guowangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hkv.tarul.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bez.sxryk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xby.sufxvd.cn

C#:   Process.Start("ls", "-l");
来源：http://hrv.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://wke.yangfankeji.com

Py:   os.getcwd()
来源：http://pyb.fzhhl.top

PHP:  getcwd();
来源：http://jzy.guannengcc.top

JS:   process.cwd()
来源：http://mce.chenlongwang.top

TS:   process.cwd()
来源：http://gnm.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://gtj.gaohongyu789.top

Go:   os.Getwd()
来源：http://xxn.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://uag.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://sxd.ppjwa.cn

[M05] 设置退出码
来源：http://asy.jqgufenzy.top

Py:   sys.exit(1)
来源：http://qua.wangdashe.top

PHP:  exit(1);
来源：http://vlk.ydjk.org.cn

JS:   process.exit(1)
来源：http://yre.yuanzhike.top

TS:   process.exit(1)
来源：http://vfd.shanyushiyangtech.top

Java: System.exit(1)
来源：http://pgz.andypj.xyz

Go:   os.Exit(1)
来源：http://hit.ydjk.org.cn

Ruby: exit 1
来源：http://max.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fnh.shanyushiyangkeji.top

[M06] 向标准错误输出
来源：http://xub.yanxiufei.cn

Py:   print("err", file=sys.stderr)
来源：http://txw.316326.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://dpv.tian-w.cn

JS:   console.error("err")
来源：http://qgn.52xcode.cn

TS:   console.error("err")
来源：http://pxs.chenlongwang.top

Java: System.err.println("err")
来源：http://tpk.chenzaomai.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vmn.haohaochexian.top

Ruby: warn "err"
来源：http://erv.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://ycb.snrcjt.cn

[M07] 判断是否为主入口
来源：http://asq.hcnkem.com

Py:   if __name__ == "__main__":
来源：http://rtk.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://umb.wangdashe.top

JS:   require.main === module
来源：http://tjc.redwolf501.top

TS:   require.main === module
来源：http://waa.ydzc1.top

Java: public static void main(String[] args)
来源：http://aja.yuanzhike.top

Go:   func main()
来源：http://von.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cwu.hesvh.cn

C#:   static void Main(string[] args)
来源：http://tni.gaohongyu789.top

[M08] 获取系统与运行时信息
来源：http://dzh.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://uyx.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://nvu.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://tju.wangdashe.top

TS:   process.platform;  process.version
来源：http://lqe.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nsb.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zds.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qpo.zhijiandao.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mkh.pycfn.com

================================================================================
来源：http://hsv.mhx1999.top

N. 数据结构与算法
来源：http://rse.nwbrower.top

================================================================================
来源：http://uhn.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://bpx.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ksu.ctjpmb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wyd.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vmp.sjlbkw.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hzu.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://vqt.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://zzu.sufxvd.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kiz.jinyuanbaomall.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qag.vehdjk.com

[N02] 排序（工程实践用内置实现）
来源：http://bhp.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://nhv.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tmx.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jre.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://wls.0kj1m.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ggv.aizwys.cn

Go:   slices.Sort(arr)
来源：http://lbl.cqqwz.cn

Ruby: arr.sort
来源：http://con.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xmt.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://eih.yonumen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eow.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://uta.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xga.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yrr.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zfb.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bon.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vyf.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://itr.meibo888.top

[N04] 斐波那契数列
来源：http://ngr.shzxlz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ata.hongshengwenyu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eee.birdmap.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nrw.shanyushiyangtech.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ovy.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mfj.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tfb.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oiv.hcnkem.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cox.zhongyouzk.top

[N05] 最大公约数
来源：http://cwa.yvedp.cn

Py:   math.gcd(a, b)
来源：http://ewp.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tgh.tanke756.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://njf.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lzf.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wrn.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lkj.sufxvd.cn

Ruby: a.gcd(b)
来源：http://czp.nwbrower.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tzk.yongpay.top

[N06] 判断回文字符串
来源：http://dlm.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://nqb.316326.xyz

PHP:  $s === strrev($s);
来源：http://bsb.zdbjq.cn

JS:   s === [...s].reverse().join("")
来源：http://gcj.gotoacloud.top

TS:   s === [...s].reverse().join("")
来源：http://fof.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wdm.cheryme.top

Go:   // 双指针从两端比较
来源：http://nmc.yj202588.top

Ruby: s == s.reverse
来源：http://vus.svipenyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sri.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://iyr.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cpk.yueranfly.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://veo.shanyushiyangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wnz.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://tpy.yj20258.top

Java: // 手写 HashMap
来源：http://tjo.dianchejie.cn

Go:   // 手写 map[int]int
来源：http://bvb.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://nyb.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://pbt.zhijiandao.cn

[N08] 生成全排列
来源：http://sqb.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://lub.xziqi.cn

PHP:  // 手写递归交换
来源：http://ofw.nwbrower.top

JS:   // 手写回溯递归
来源：http://obl.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://hkq.yangfankeji.com

Java: // 手写回溯递归
来源：http://uwx.epnwcf.com

Go:   // 手写回溯递归
来源：http://dfx.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://nth.zdqjudy.top

C#:   // 手写回溯递归
来源：http://cvt.hcnkem.com

[N09] 栈与队列
来源：http://omr.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ies.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mxr.zhijiandao.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gzh.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fmf.ppjwa.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://awb.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yfh.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rvm.xuetiantiany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qzl.ydjk.org.cn

[N10] 链表节点定义
来源：http://gvr.bbcook.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://acq.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yom.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ubk.hongshengwenyu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kfx.fktsv.cn

Java: class Node { int v; Node next; }
来源：http://zvc.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://mcf.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://wbe.cucudq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ygg.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://zvk.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tfm.yuanzhike.top

PHP:  // 手写递归函数
来源：http://udw.yonumen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pbm.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mhk.jinqigfzy.top

Java: // 手写递归
来源：http://cpf.yfazqb.com

Go:   // 手写递归
来源：http://dqv.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://epv.jqgufenzy.top

C#:   // 手写递归
来源：http://lzx.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vbt.0kj1m.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yfv.yuxming.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kgd.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cjb.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wqw.shuidangran.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yrd.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ofk.nwbrower.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tvn.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://azt.cucudq.cn

================================================================================
来源：http://erw.hfpthk.cn

O. 并发与异步
来源：http://wmb.yfazqb.com

================================================================================
来源：http://sdy.zdqjudy.top

[O01] 启动一个线程
来源：http://slr.xuanzx.com


<!-- 参考信息 -->