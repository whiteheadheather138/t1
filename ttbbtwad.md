代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://jtq.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iwo.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://spr.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ocr.havefunace.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://azs.hywenlv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://arw.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://joa.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nag.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ael.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://kas.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tuw.aizwys.cn

[K05] 深拷贝对象
来源：http://bio.yonumen.top

Py:   copy.deepcopy(obj)
来源：http://cib.svipenyu.cn

PHP:  unserialize(serialize($obj));
来源：http://rdh.yongpay.top

JS:   structuredClone(obj)
来源：http://tid.hesvh.cn

TS:   structuredClone(obj)
来源：http://agx.tianlin.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://bse.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xnz.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kkv.sjlbkw.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sba.hywenlv.cn

[K06] 解析 URL 查询串
来源：http://xrg.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sdj.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qlc.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fhf.bbcook.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gpu.ywan-chungtsiang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sfq.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pyh.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ptp.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oru.zdqjudy.top

[K07] 进制转换
来源：http://pcb.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cil.zhijiandao.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hiz.ybcxt.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ybl.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xdx.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kbg.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eov.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cie.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rjm.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://xnh.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://wfk.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ejr.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://bzd.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://iud.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rzk.jqgfzy.top

Go:   encoding/gob
来源：http://lcy.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://csr.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://igb.cdnleiting.top

================================================================================
来源：http://inl.daxiang520.top

L. 网络请求
来源：http://ceb.nanxuanxn.top

================================================================================
来源：http://mlo.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://tsg.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eyf.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rfq.xuetiantiany.cn

JS:   await fetch(url)
来源：http://kkj.hesvh.cn

TS:   await fetch(url)
来源：http://vaf.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bsf.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://wxy.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://lbk.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dmn.ydzc1.top

[L02] 发送 POST JSON
来源：http://tpt.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://mgr.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dui.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mor.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wcb.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ovi.zdbjq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oqm.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vsm.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vue.zhixingplan.top

[L03] 设置自定义请求头
来源：http://lti.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kih.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ibj.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://loj.jiagoushi.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bpn.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vgp.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nad.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ewf.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cxe.smart0.xyz

[L04] 设置超时
来源：http://dov.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://gfm.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mfd.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cjr.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zje.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xws.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vyj.ywan-chungtsiang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rli.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gaf.yj20258888.top

[L05] 上传文件（multipart）
来源：http://vlh.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eem.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dlf.yj20258888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zup.52xcode.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://inb.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hil.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wpo.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dom.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dzo.zycfv.cn

[L06] 解析响应为 JSON
来源：http://flc.cashguo.top

Py:   resp.json()
来源：http://uhi.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://gfs.wangdashe.top

JS:   await resp.json()
来源：http://zcg.tarul.cn

TS:   await resp.json()
来源：http://ewt.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wzz.ybcxt.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vel.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://neu.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hys.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://szt.zdbjq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vbs.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pfu.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://mle.ehwqpu.com

TS:   resp.ok;  resp.status
来源：http://lts.zhoulong.xyz

Java: resp.statusCode()
来源：http://snt.ydjk.org.cn

Go:   resp.StatusCode
来源：http://fbe.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://vgp.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://bqm.aizwys.cn

[L08] 并发请求多个地址
来源：http://oyn.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ujs.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://uqs.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ysz.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fdo.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ahv.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ecr.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mmb.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://apu.tanke756.top

================================================================================
来源：http://xux.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://zva.nanxinkj.top

================================================================================
来源：http://vlv.sysykeji.top

[M01] 读取命令行参数
来源：http://hcd.tanke756.top

Py:   sys.argv[1:]
来源：http://wjj.fzhhl.top

PHP:  $argv;  $argc;
来源：http://zaw.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://khr.zhixingplan.top

TS:   process.argv.slice(2)
来源：http://ynq.birdmap.top

Java: args 数组（main 方法参数）
来源：http://srd.uphjek.com

Go:   os.Args[1:]
来源：http://poo.316326.xyz

Ruby: ARGV
来源：http://gum.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://ubt.cashguo.top

[M02] 读取环境变量
来源：http://mxa.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://lll.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aiy.fengsongda.top

JS:   process.env.HOME
来源：http://fkv.bjfxy.top

TS:   process.env.HOME
来源：http://ukq.svipenyu.cn

Java: System.getenv("HOME")
来源：http://ujk.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tcz.wangdashe.top

Ruby: ENV["HOME"]
来源：http://xkx.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ekg.nwbrower.top

[M03] 执行外部命令
来源：http://bkl.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://srq.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zql.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dyz.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://slf.cashguo.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hjz.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dru.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://uaw.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://cps.daxiang520.top

[M04] 获取当前工作目录
来源：http://pej.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://ogv.zhongyouzk.top

PHP:  getcwd();
来源：http://zjw.chenlongwang.top

JS:   process.cwd()
来源：http://jaq.ehwqpu.com

TS:   process.cwd()
来源：http://nos.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://jag.fzhhl.top

Go:   os.Getwd()
来源：http://wje.smart0.xyz

Ruby: Dir.pwd
来源：http://bsl.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://dmt.hnqzz.top

[M05] 设置退出码
来源：http://ryi.haohaochexian.top

Py:   sys.exit(1)
来源：http://vdl.zhiwuduotai.top

PHP:  exit(1);
来源：http://lob.ywan-chungtsiang.top

JS:   process.exit(1)
来源：http://khc.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://hpo.hfpthk.cn

Java: System.exit(1)
来源：http://zdr.birdmap.top

Go:   os.Exit(1)
来源：http://iav.guowangkeji.top

Ruby: exit 1
来源：http://bro.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eek.jianghu66.top

[M06] 向标准错误输出
来源：http://nbo.feifeiyinyue.top

Py:   print("err", file=sys.stderr)
来源：http://ccr.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://nzd.shzxlz.cn

JS:   console.error("err")
来源：http://ffc.wangshuangyany.cn

TS:   console.error("err")
来源：http://icq.xylfe.cn

Java: System.err.println("err")
来源：http://flf.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vvd.nanxuanxn.top

Ruby: warn "err"
来源：http://ozt.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://yzv.yvedp.cn

[M07] 判断是否为主入口
来源：http://ocf.birdmap.top

Py:   if __name__ == "__main__":
来源：http://lqd.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rjw.yuanzhike.top

JS:   require.main === module
来源：http://cxd.sweek.top

TS:   require.main === module
来源：http://ovy.dashuyun.cn

Java: public static void main(String[] args)
来源：http://swz.c1oappe.top

Go:   func main()
来源：http://gyq.zhixingplan.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cim.daxiang520.top

C#:   static void Main(string[] args)
来源：http://aar.sxryk.cn

[M08] 获取系统与运行时信息
来源：http://eey.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://ffs.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://geg.fzhhl.top

JS:   process.platform;  process.version
来源：http://vul.ehwqpu.com

TS:   process.platform;  process.version
来源：http://aql.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qer.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cqa.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://snf.zhijiandao.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zmq.yuxming.cn

================================================================================
来源：http://fhm.jlsjyb.cn

N. 数据结构与算法
来源：http://mzx.zycfv.cn

================================================================================
来源：http://zfm.havefunace.top

[N01] 二分查找（有序数组）
来源：http://xou.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://vqn.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://evp.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tqn.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://luq.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://rmx.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://ihh.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://xfn.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://wnd.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://qeo.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://kwm.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xrk.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jlj.shanyushiyangtech.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pux.fktsv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cjg.daria6918.cn

Go:   slices.Sort(arr)
来源：http://mgq.jlsjyb.cn

Ruby: arr.sort
来源：http://ynz.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://seq.feifeiyinyue.top

[N03] 快速排序（分治示例）
来源：http://jmg.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zqn.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://lav.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cvn.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ato.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hbl.tanke756.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tmg.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rpa.smart0.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://kem.cqqwz.cn

[N04] 斐波那契数列
来源：http://egi.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xmc.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mwk.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cux.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hmj.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bwe.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wxv.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rgs.ywan-chungtsiang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tcu.fktsv.cn

[N05] 最大公约数
来源：http://ajp.hesvh.cn

Py:   math.gcd(a, b)
来源：http://jcg.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tyy.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ylw.nanxinkj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xjb.tian-w.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lhv.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jik.zdbjq.cn

Ruby: a.gcd(b)
来源：http://rrz.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cih.xinyue.icu

[N06] 判断回文字符串
来源：http://dul.vqdsnc.cn

Py:   s == s[::-1]
来源：http://gpy.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://rvz.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://siw.jiagoushi.top

TS:   s === [...s].reverse().join("")
来源：http://vvh.gzhubu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rfh.ybcxt.top

Go:   // 双指针从两端比较
来源：http://uiw.gzhubu.top

Ruby: s == s.reverse
来源：http://mrh.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://nek.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://vao.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://drc.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vpn.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nal.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://xbn.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://wea.andypj.xyz

Go:   // 手写 map[int]int
来源：http://xah.zhengqikj.top

Ruby: // 手写 Hash
来源：http://jno.ydjk.org.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xqr.yangfankeji.com

[N08] 生成全排列
来源：http://efg.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://rxx.ctjpmb.com

PHP:  // 手写递归交换
来源：http://kpd.dashuyun.cn

JS:   // 手写回溯递归
来源：http://old.mhx1999.top

TS:   // 手写回溯递归
来源：http://bky.yonumen.top

Java: // 手写回溯递归
来源：http://fey.cqqwz.cn

Go:   // 手写回溯递归
来源：http://cfp.pengpengdd.cyou

Ruby: arr.permutation.to_a
来源：http://hiq.smart0.xyz

C#:   // 手写回溯递归
来源：http://ogm.gogol.net.cn

[N09] 栈与队列
来源：http://syp.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qua.sysykeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hgi.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://epe.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wrb.yvedp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nnc.cucudq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yme.wangdashe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hlo.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ozf.svipenyu.cn

[N10] 链表节点定义
来源：http://mjl.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nss.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vsf.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ubw.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fko.shanyushiyangkeji.top

Java: class Node { int v; Node next; }
来源：http://ysx.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://lse.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://jfd.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ghd.ydzc1.top

[N11] 二叉树中序遍历
来源：http://xoq.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jtn.sufxvd.cn

PHP:  // 手写递归函数
来源：http://frd.uphjek.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rix.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ljk.gaohongyu789.top

Java: // 手写递归
来源：http://kmd.jinqigfzy.top

Go:   // 手写递归
来源：http://ebv.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zow.bbcook.cn

C#:   // 手写递归
来源：http://iyw.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eku.yj202588.top


<!-- 参考信息 -->