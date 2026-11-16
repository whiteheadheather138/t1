代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://ydo.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qdp.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rjf.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bcb.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://qaf.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://biw.yongpay.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://amv.nanxinkj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jpt.yj20258.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dwo.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wln.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xjv.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ody.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wsz.yj20258.top

[K07] 进制转换
来源：http://pqe.tarul.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lng.yongpay.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qdw.yueranfly.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oug.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gzm.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://znh.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bij.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pbg.vqdsnc.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wjn.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://lnr.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://qfv.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aye.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://yji.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://ilz.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ekz.snrcjt.cn

Go:   encoding/gob
来源：http://hua.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://uog.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vqc.wangdashe.top

================================================================================
来源：http://seu.zhiwuduotai.top

L. 网络请求
来源：http://hkv.zhaomingkeji.xyz

================================================================================
来源：http://wzj.yj20258.top

[L01] 发送 GET 请求
来源：http://dzp.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vwe.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iyd.sweek.top

JS:   await fetch(url)
来源：http://eoo.zdqjudy.top

TS:   await fetch(url)
来源：http://nzh.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xyk.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://lmn.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://uyy.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jai.hcnkem.com

[L02] 发送 POST JSON
来源：http://urn.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://wto.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oji.yuanzhike.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vlw.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uxw.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cej.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bvg.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yjf.wangshuangyany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dpy.hcnkem.com

[L03] 设置自定义请求头
来源：http://uqx.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bkh.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zij.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wtl.fengsongda.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://spk.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jwz.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bwa.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dxv.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qqx.kuanghao11.cn

[L04] 设置超时
来源：http://riw.xinyue.icu

Py:   requests.get(url, timeout=5)
来源：http://yay.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://izp.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zbs.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wmi.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mkt.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dhj.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mmf.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ety.tianlin.xyz

[L05] 上传文件（multipart）
来源：http://ndr.yj20258888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nls.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sxu.smart0.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vgr.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ogj.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vjg.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://upj.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gka.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vhu.birdmap.top

[L06] 解析响应为 JSON
来源：http://itb.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://ukh.yvedp.cn

PHP:  json_decode($body, true);
来源：http://spm.wangshuangyany.cn

JS:   await resp.json()
来源：http://bdf.zhiwuduotai.top

TS:   await resp.json()
来源：http://ith.uphjek.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hkw.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bas.pengpengdd.cyou

Ruby: JSON.parse(resp.body)
来源：http://alf.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qib.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://ffv.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://amt.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gij.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://lil.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://hbk.cashguo.top

Java: resp.statusCode()
来源：http://xfa.jianghu66.top

Go:   resp.StatusCode
来源：http://ljb.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://ury.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://cbt.fehbvm.com

[L08] 并发请求多个地址
来源：http://qrn.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://okj.guowangkeji.top

PHP:  curl_multi_init() 系列
来源：http://qyn.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qda.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://brn.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://emu.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zkh.smart0.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://edc.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pax.yj20258888.top

================================================================================
来源：http://ecp.ppjwa.cn

M. 命令行 / 进程 / 环境
来源：http://bag.vehdjk.com

================================================================================
来源：http://wqc.tarul.cn

[M01] 读取命令行参数
来源：http://mgq.hfpthk.cn

Py:   sys.argv[1:]
来源：http://ktr.bjfxy.top

PHP:  $argv;  $argc;
来源：http://ywy.meibo888.top

JS:   process.argv.slice(2)
来源：http://pyu.ybcxt.top

TS:   process.argv.slice(2)
来源：http://wfp.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://sgp.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://cex.zhoulong.xyz

Ruby: ARGV
来源：http://rxa.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://qts.cucudq.cn

[M02] 读取环境变量
来源：http://eok.hywenlv.cn

Py:   os.environ.get("HOME")
来源：http://aaa.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://htx.meibo888.top

JS:   process.env.HOME
来源：http://zjd.sufxvd.cn

TS:   process.env.HOME
来源：http://tiq.zhoulong.xyz

Java: System.getenv("HOME")
来源：http://vfa.nwbrower.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://efw.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://lca.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zrp.hongshengwenyu.top

[M03] 执行外部命令
来源：http://iwg.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fzh.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dof.zhongyouzk.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wjq.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nxp.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nzm.shuidangran.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qiq.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://idc.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://hxj.uphjek.com

[M04] 获取当前工作目录
来源：http://xmp.havefunace.top

Py:   os.getcwd()
来源：http://gnj.bbcook.cn

PHP:  getcwd();
来源：http://rei.feifeiyinyue.top

JS:   process.cwd()
来源：http://coq.svipenyu.cn

TS:   process.cwd()
来源：http://pgc.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://lhk.epnwcf.com

Go:   os.Getwd()
来源：http://cit.andypj.xyz

Ruby: Dir.pwd
来源：http://jwo.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://avw.zhiwuduotai.top

[M05] 设置退出码
来源：http://iyr.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://wst.yueranfly.top

PHP:  exit(1);
来源：http://acw.smart0.xyz

JS:   process.exit(1)
来源：http://boi.ivvv.top

TS:   process.exit(1)
来源：http://nut.aizwys.cn

Java: System.exit(1)
来源：http://clv.vehdjk.com

Go:   os.Exit(1)
来源：http://myp.aibaodan.cn

Ruby: exit 1
来源：http://zei.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dyc.pengpengdd.cyou

[M06] 向标准错误输出
来源：http://odn.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://mtc.aizwys.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tae.yuxming.cn

JS:   console.error("err")
来源：http://oen.hnxiangtu.top

TS:   console.error("err")
来源：http://trw.fehbvm.com

Java: System.err.println("err")
来源：http://hyz.fktsv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wjf.tianlin.xyz

Ruby: warn "err"
来源：http://ykd.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://hxf.chenzaomai.com

[M07] 判断是否为主入口
来源：http://rzd.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://mbc.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://juk.mhx1999.top

JS:   require.main === module
来源：http://fxq.sysykeji.top

TS:   require.main === module
来源：http://rsj.aibaodan.cn

Java: public static void main(String[] args)
来源：http://bcl.cheryme.top

Go:   func main()
来源：http://enq.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kxb.hesvh.cn

C#:   static void Main(string[] args)
来源：http://rce.sweek.top

[M08] 获取系统与运行时信息
来源：http://ofv.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://tae.tian-w.cn

PHP:  PHP_OS;  phpversion();
来源：http://jqq.epnwcf.com

JS:   process.platform;  process.version
来源：http://uti.shanyushiyangtech.top

TS:   process.platform;  process.version
来源：http://aek.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uxi.jinyuanbaomall.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ptj.aizwys.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://stz.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://llc.sysykeji.top

================================================================================
来源：http://rcr.xuetiantiany.cn

N. 数据结构与算法
来源：http://lzs.xuanzx.com

================================================================================
来源：http://vwf.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://kgm.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://dkp.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gcf.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ghk.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iuh.hcnkem.com

Java: Arrays.binarySearch(arr, x)
来源：http://xih.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://oxm.316326.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://hsl.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://eda.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://hzo.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://kvv.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dqs.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uof.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://god.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oin.yj20258.top

Go:   slices.Sort(arr)
来源：http://voh.cucudq.cn

Ruby: arr.sort
来源：http://lla.hysaishi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rpg.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://rje.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://miq.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://uvv.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://neb.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mwx.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ura.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bll.yueranfly.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tkh.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://dwb.pycfn.com

[N04] 斐波那契数列
来源：http://vfk.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xpk.wangdashe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xml.tianlin.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://frp.gotoacloud.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lpn.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aof.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lww.birdmap.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ztl.guowangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kck.birdmap.top

[N05] 最大公约数
来源：http://vhf.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://xcx.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://orz.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cbi.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sne.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mtk.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xhs.yonumen.top

Ruby: a.gcd(b)
来源：http://lry.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vtn.sysykeji.top

[N06] 判断回文字符串
来源：http://gkd.cashguo.top

Py:   s == s[::-1]
来源：http://vox.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://wys.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://mrb.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://nfd.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yvw.meibo888.top

Go:   // 双指针从两端比较
来源：http://vyv.cqqwz.cn

Ruby: s == s.reverse
来源：http://oor.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://qhl.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://sdi.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sqk.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yon.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://edj.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://ngv.sjlbkw.cn

Java: // 手写 HashMap
来源：http://sdw.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://exx.jianghu66.top

Ruby: // 手写 Hash
来源：http://vny.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://miy.sufxvd.cn

[N08] 生成全排列
来源：http://bsv.hammf.cn

Py:   itertools.permutations(arr)
来源：http://sng.ydzc1.top

PHP:  // 手写递归交换
来源：http://ylm.zhengqikj.top

JS:   // 手写回溯递归
来源：http://qjf.cashguo.top

TS:   // 手写回溯递归
来源：http://hps.jyoumei.cn

Java: // 手写回溯递归
来源：http://fwx.birdmap.top

Go:   // 手写回溯递归
来源：http://zth.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://iup.havefunace.top

C#:   // 手写回溯递归
来源：http://dtw.zhixingplan.top

[N09] 栈与队列
来源：http://tzb.uphjek.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hpu.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bho.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gnd.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ale.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zby.nanxuanxn.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ixy.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cdy.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tfo.ehwqpu.com

[N10] 链表节点定义
来源：http://ssg.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xih.9152youxi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cex.gogol.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ryz.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ska.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://jks.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://yab.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://bmu.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lfr.fktsv.cn

[N11] 二叉树中序遍历
来源：http://xkb.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ath.ydzc1.top

PHP:  // 手写递归函数
来源：http://hxn.daria6918.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mjs.9152youxi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cnu.sysykeji.top

Java: // 手写递归
来源：http://xgl.52xcode.cn

Go:   // 手写递归
来源：http://kdc.yj202588.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bzw.mhx1999.top

C#:   // 手写递归
来源：http://qzj.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wxu.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kre.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rqh.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jmj.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://htr.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xhi.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ovm.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wiw.sysykeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ezn.cdnleiting.top

================================================================================
来源：http://yyc.dashuyun.cn

O. 并发与异步
来源：http://crx.jqgufenzy.top

================================================================================
来源：http://pkt.smart0.xyz

[O01] 启动一个线程
来源：http://wzl.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xqp.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fca.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://irj.gaohongyu789.top

TS:   // 同 JS
来源：http://nsw.xuanzx.com


<!-- 参考信息 -->