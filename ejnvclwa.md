代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lpg.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jxi.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iqw.gogol.net.cn

[K05] 深拷贝对象
来源：http://ems.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://kca.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://vxx.jqgfzy.top

JS:   structuredClone(obj)
来源：http://nfp.chenzaomai.com

TS:   structuredClone(obj)
来源：http://zvs.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rlz.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://opf.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xro.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kcb.pengpengdd.cyou

[K06] 解析 URL 查询串
来源：http://tii.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cdy.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xep.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wit.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://awc.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://etq.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://amj.hongshengwenyu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nvu.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://otf.xuanzx.com

[K07] 进制转换
来源：http://sxw.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gqw.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ihw.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nsp.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sff.smart0.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://odu.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xbg.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kal.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gdr.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://vlp.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://yat.fengsongda.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iei.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://aix.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://qaj.iojbl.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ywh.cdnleiting.top

Go:   encoding/gob
来源：http://iup.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://rtg.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tmo.jinghuilouyu.cn

================================================================================
来源：http://gmw.cucudq.cn

L. 网络请求
来源：http://xxs.sysykeji.top

================================================================================
来源：http://eue.sufxvd.cn

[L01] 发送 GET 请求
来源：http://slj.guannengcc.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wqz.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pam.zhongyouzk.top

JS:   await fetch(url)
来源：http://qod.snrcjt.cn

TS:   await fetch(url)
来源：http://gcb.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://thv.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://yem.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://rjc.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vtn.yanxiufei.cn

[L02] 发送 POST JSON
来源：http://vpb.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://fqk.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hkp.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hmz.guowangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tit.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nlj.52xcode.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ugr.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vos.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nak.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://kbm.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jrj.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dlg.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fls.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tch.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bkm.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pfh.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ohd.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dax.ybcxt.top

[L04] 设置超时
来源：http://tir.zhijiandao.cn

Py:   requests.get(url, timeout=5)
来源：http://jsv.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xjc.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ixt.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bjr.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yhn.fzhhl.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ztg.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ukc.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vgt.cucudq.cn

[L05] 上传文件（multipart）
来源：http://cbp.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kjx.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tkv.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ggk.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pbz.hammf.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ipo.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lyj.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fjl.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bgg.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://xpl.jinqigufen.top

Py:   resp.json()
来源：http://vnl.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://evp.iojbl.cn

JS:   await resp.json()
来源：http://hos.chenzaomai.com

TS:   await resp.json()
来源：http://cli.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rfv.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zte.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://uvg.xylfe.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fhe.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://vze.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pvg.tanke756.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://erq.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://jbm.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://thh.gogol.net.cn

Java: resp.statusCode()
来源：http://vzq.zhixingplan.top

Go:   resp.StatusCode
来源：http://bqw.feifeiyinyue.top

Ruby: resp.code.to_i
来源：http://bpq.yj20258.top

C#:   (int)resp.StatusCode
来源：http://ynn.redwolf501.top

[L08] 并发请求多个地址
来源：http://obi.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wvs.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://qdf.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pao.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zni.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qnb.fanxiaobao.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ukt.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xuv.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tmw.ywan-chungtsiang.top

================================================================================
来源：http://jor.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://yer.quarkkingdee.top

================================================================================
来源：http://ium.nwbrower.top

[M01] 读取命令行参数
来源：http://txz.ctjpmb.com

Py:   sys.argv[1:]
来源：http://dpc.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://qzp.aizwys.cn

JS:   process.argv.slice(2)
来源：http://kzg.daria6918.cn

TS:   process.argv.slice(2)
来源：http://kvn.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://fde.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://tyc.jinqigfzy.top

Ruby: ARGV
来源：http://uyk.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://qyi.hywenlv.cn

[M02] 读取环境变量
来源：http://yrz.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://ytu.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://icl.smart0.xyz

JS:   process.env.HOME
来源：http://zft.birdmap.top

TS:   process.env.HOME
来源：http://ukk.jinqigufen.top

Java: System.getenv("HOME")
来源：http://rsu.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bdn.daxiang520.top

Ruby: ENV["HOME"]
来源：http://roh.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zkj.yonumen.top

[M03] 执行外部命令
来源：http://hpu.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ssi.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zbu.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://izt.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iui.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qdb.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jig.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://usf.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://swj.aizwys.cn

[M04] 获取当前工作目录
来源：http://skq.fanxiaobao.xyz

Py:   os.getcwd()
来源：http://kad.feifeiyinyue.top

PHP:  getcwd();
来源：http://fzk.ybcxt.top

JS:   process.cwd()
来源：http://qjz.sweek.top

TS:   process.cwd()
来源：http://mpk.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://ljm.kuanghao11.cn

Go:   os.Getwd()
来源：http://ori.gzhubu.top

Ruby: Dir.pwd
来源：http://oof.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://own.zhengqikj.top

[M05] 设置退出码
来源：http://epf.jyoumei.cn

Py:   sys.exit(1)
来源：http://qjm.xylfe.cn

PHP:  exit(1);
来源：http://hyx.zhiwuduotai.top

JS:   process.exit(1)
来源：http://ktv.zdbjq.cn

TS:   process.exit(1)
来源：http://kvg.feifeiyinyue.top

Java: System.exit(1)
来源：http://zcj.mhx1999.top

Go:   os.Exit(1)
来源：http://pju.jqgfzy.top

Ruby: exit 1
来源：http://azx.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fyh.hammf.cn

[M06] 向标准错误输出
来源：http://hiu.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://vsn.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zau.zycfv.cn

JS:   console.error("err")
来源：http://dul.sweek.top

TS:   console.error("err")
来源：http://fvd.wangdashe.top

Java: System.err.println("err")
来源：http://bkc.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cxk.cashguo.top

Ruby: warn "err"
来源：http://yvm.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://izf.fzhhl.top

[M07] 判断是否为主入口
来源：http://bxq.tarul.cn

Py:   if __name__ == "__main__":
来源：http://ayo.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://orv.shangyingyoupin.top

JS:   require.main === module
来源：http://haz.svipenyu.cn

TS:   require.main === module
来源：http://nqn.birdmap.top

Java: public static void main(String[] args)
来源：http://mnn.wangshuangyany.cn

Go:   func main()
来源：http://pur.hfpthk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kmp.yongpay.top

C#:   static void Main(string[] args)
来源：http://ptb.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://huy.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://nwe.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://dmq.havefunace.top

JS:   process.platform;  process.version
来源：http://edo.shuidangran.top

TS:   process.platform;  process.version
来源：http://ceh.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ckv.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hqi.yanxiufei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kyd.uphjek.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://zkk.bbcook.cn

================================================================================
来源：http://lwv.fzhhl.top

N. 数据结构与算法
来源：http://bgu.zdbjq.cn

================================================================================
来源：http://jht.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://tii.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zto.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://znj.yongpay.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lyh.hnxiangtu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vaa.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://qtm.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://cxa.sufxvd.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xhj.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iqw.xingfuxueyuan.xyz

[N02] 排序（工程实践用内置实现）
来源：http://dmc.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://qqr.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tum.jiagoushi.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xqg.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rmt.52xcode.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://voe.zhijiandao.cn

Go:   slices.Sort(arr)
来源：http://ywd.wangdashe.top

Ruby: arr.sort
来源：http://vfy.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gjg.fanxiaobao.xyz

[N03] 快速排序（分治示例）
来源：http://pui.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gqy.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://wkf.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jrb.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://voe.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rym.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nrj.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cbq.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://etx.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://jpj.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hxt.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hpz.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dlh.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ken.jqgfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qmz.cheryme.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ooe.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vbw.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yne.sjlbkw.cn

[N05] 最大公约数
来源：http://voj.yongpay.top

Py:   math.gcd(a, b)
来源：http://mac.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ufd.wangdashe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mxg.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rqf.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://grt.ctjpmb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pfd.zdbjq.cn

Ruby: a.gcd(b)
来源：http://qqa.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://glf.tianlin.xyz

[N06] 判断回文字符串
来源：http://lkn.aibaodan.cn

Py:   s == s[::-1]
来源：http://slb.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://dxz.cheryme.top

JS:   s === [...s].reverse().join("")
来源：http://rdf.cucudq.cn

TS:   s === [...s].reverse().join("")
来源：http://epf.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jwy.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://sdq.shuidangran.top

Ruby: s == s.reverse
来源：http://gcs.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wfl.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://sji.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ubj.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qpx.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://xld.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://gvd.hammf.cn

Java: // 手写 HashMap
来源：http://ooy.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://sxu.yonumen.top

Ruby: // 手写 Hash
来源：http://zqv.ybcxt.top

C#:   // 手写 Dictionary<int, int>
来源：http://lsk.hammf.cn

[N08] 生成全排列
来源：http://xdn.pycfn.com

Py:   itertools.permutations(arr)
来源：http://piv.316326.xyz

PHP:  // 手写递归交换
来源：http://xfb.chenlongwang.top

JS:   // 手写回溯递归
来源：http://ong.andypj.xyz

TS:   // 手写回溯递归
来源：http://zko.gaohongyu789.top

Java: // 手写回溯递归
来源：http://ykf.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://hlb.cashguo.top

Ruby: arr.permutation.to_a
来源：http://onw.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://jgg.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://iuv.zycfv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vwb.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dqe.chenlongwang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://doh.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tyf.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gqh.sysykeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ryw.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kih.vqdsnc.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kja.jinqigfzy.top

[N10] 链表节点定义
来源：http://rzb.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hvg.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://col.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ijs.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rno.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://leb.zhaomingkeji.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://jce.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bjf.zhaomingkeji.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://vix.yfazqb.com

[N11] 二叉树中序遍历
来源：http://gnw.9152youxi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jrj.hysaishi.cn

PHP:  // 手写递归函数
来源：http://yzb.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://skc.ppjwa.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wug.ydzc1.top

Java: // 手写递归
来源：http://jmw.sufxvd.cn

Go:   // 手写递归
来源：http://afu.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xqz.iojbl.cn

C#:   // 手写递归
来源：http://otq.wangshuangyany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ofc.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ccp.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gmu.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tcq.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tua.ydzc1.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iqa.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://axg.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ovc.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gtq.hcnkem.com


<!-- 参考信息 -->