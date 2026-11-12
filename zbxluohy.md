代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://wiy.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://idp.tian-w.cn

[K04] 读取 JSON 文件
来源：http://asp.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dts.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bpe.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rvc.jlsjyb.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zhz.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sqo.dianchejie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ytp.ydzc1.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bdr.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xai.birdmap.top

[K05] 深拷贝对象
来源：http://jzf.jinghuilouyu.cn

Py:   copy.deepcopy(obj)
来源：http://ani.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://sgd.cheryme.top

JS:   structuredClone(obj)
来源：http://fwh.snrcjt.cn

TS:   structuredClone(obj)
来源：http://cgn.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kar.yueranfly.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xwc.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rnp.fzhhl.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nzt.ydzc1.top

[K06] 解析 URL 查询串
来源：http://uot.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dos.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bxu.jiagoushi.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kjx.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qtr.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sml.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nyi.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rfx.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kdw.ehwqpu.com

[K07] 进制转换
来源：http://qqk.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jul.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bam.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zlh.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://spj.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nmo.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gyx.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aov.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fcb.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://vky.hammf.cn

Py:   pickle.dumps(obj)
来源：http://mlv.cheryme.top

PHP:  serialize($obj);  unserialize($s);
来源：http://umx.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://sau.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://mju.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fbi.yongpay.top

Go:   encoding/gob
来源：http://wow.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://mmr.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vkw.zycfv.cn

================================================================================
来源：http://kwn.jyoumei.cn

L. 网络请求
来源：http://axv.sufxvd.cn

================================================================================
来源：http://tnp.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://mju.vqdsnc.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ruz.andypj.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mnm.zhongyouzk.top

JS:   await fetch(url)
来源：http://hqb.aizwys.cn

TS:   await fetch(url)
来源：http://jme.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xnd.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://zzf.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pcu.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://naf.hysaishi.cn

[L02] 发送 POST JSON
来源：http://alx.sufxvd.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lzg.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mly.hywenlv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wqp.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lof.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://upd.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qlb.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bja.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tyf.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://wbq.yanxiufei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hwd.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tjy.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hwl.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tsc.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hcf.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sxi.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dzr.uphjek.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iqw.fktsv.cn

[L04] 设置超时
来源：http://umg.zhongyouzk.top

Py:   requests.get(url, timeout=5)
来源：http://gtu.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wll.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rbs.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xvx.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://stz.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nqc.hnxiangtu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yjb.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nbx.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://epz.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zzg.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kbh.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qim.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kak.yongpay.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uyt.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fcy.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xdg.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gox.hnqzz.top

[L06] 解析响应为 JSON
来源：http://mst.nanxinkj.top

Py:   resp.json()
来源：http://ajh.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://rel.ivvv.top

JS:   await resp.json()
来源：http://zud.shangyingyoupin.top

TS:   await resp.json()
来源：http://sxx.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kui.ydzc1.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ytz.9152youxi.cn

Ruby: JSON.parse(resp.body)
来源：http://iym.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vqd.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://awp.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://itk.ivvv.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xcs.zhongyouzk.top

JS:   resp.ok;  resp.status
来源：http://uiu.yongpay.top

TS:   resp.ok;  resp.status
来源：http://ugm.chenlongwang.top

Java: resp.statusCode()
来源：http://auo.ivvv.top

Go:   resp.StatusCode
来源：http://lqq.0kj1m.cn

Ruby: resp.code.to_i
来源：http://qog.yj20258888.top

C#:   (int)resp.StatusCode
来源：http://xtu.vehdjk.com

[L08] 并发请求多个地址
来源：http://kmr.sysykeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blu.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://ijx.xuetiantiany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ajm.zhoulong.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pte.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hod.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ozv.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wis.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wiu.nanxinkj.top

================================================================================
来源：http://nrd.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://cxj.zhaomingkeji.xyz

================================================================================
来源：http://jim.fktsv.cn

[M01] 读取命令行参数
来源：http://bhh.uphjek.com

Py:   sys.argv[1:]
来源：http://hiw.kuanghao11.cn

PHP:  $argv;  $argc;
来源：http://dml.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://isw.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://tyx.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://ynx.daria6918.cn

Go:   os.Args[1:]
来源：http://zrh.zhengqikj.top

Ruby: ARGV
来源：http://mpk.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://zko.c1oappe.top

[M02] 读取环境变量
来源：http://mrp.andypj.xyz

Py:   os.environ.get("HOME")
来源：http://csg.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gpi.iojbl.cn

JS:   process.env.HOME
来源：http://vbq.vehdjk.com

TS:   process.env.HOME
来源：http://wzr.sysykeji.top

Java: System.getenv("HOME")
来源：http://ugi.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eqg.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://jtu.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eit.xuanzx.com

[M03] 执行外部命令
来源：http://zzt.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vpw.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ncn.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hgr.nwbrower.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zks.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xwb.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://scb.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://afa.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://wir.wangdashe.top

[M04] 获取当前工作目录
来源：http://fdz.nanxuanxn.top

Py:   os.getcwd()
来源：http://uxm.ppjwa.cn

PHP:  getcwd();
来源：http://spm.yvedp.cn

JS:   process.cwd()
来源：http://whj.guannengcc.top

TS:   process.cwd()
来源：http://krr.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://uwc.chenzaomai.com

Go:   os.Getwd()
来源：http://flm.zycfv.cn

Ruby: Dir.pwd
来源：http://ofe.yuanzhike.top

C#:   Directory.GetCurrentDirectory()
来源：http://mxk.sjlbkw.cn

[M05] 设置退出码
来源：http://wqj.vehdjk.com

Py:   sys.exit(1)
来源：http://abb.yueranfly.top

PHP:  exit(1);
来源：http://wdb.hnqzz.top

JS:   process.exit(1)
来源：http://tbm.vehdjk.com

TS:   process.exit(1)
来源：http://psc.mhx1999.top

Java: System.exit(1)
来源：http://gue.bjfxy.top

Go:   os.Exit(1)
来源：http://zpu.sxryk.cn

Ruby: exit 1
来源：http://nwc.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kgu.hfpthk.cn

[M06] 向标准错误输出
来源：http://qmh.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://ajw.ybcxt.top

PHP:  fwrite(STDERR, "err\n");
来源：http://chd.xziqi.cn

JS:   console.error("err")
来源：http://fra.andypj.xyz

TS:   console.error("err")
来源：http://afy.xinyue.icu

Java: System.err.println("err")
来源：http://uau.xingfuxueyuan.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tnc.zhengqikj.top

Ruby: warn "err"
来源：http://vom.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://qnd.jianghu66.top

[M07] 判断是否为主入口
来源：http://fty.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://jgx.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uoh.bbcook.cn

JS:   require.main === module
来源：http://uea.yanxiufei.cn

TS:   require.main === module
来源：http://yyr.yonumen.top

Java: public static void main(String[] args)
来源：http://rro.cucudq.cn

Go:   func main()
来源：http://vua.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://miq.vehdjk.com

C#:   static void Main(string[] args)
来源：http://mbv.hywenlv.cn

[M08] 获取系统与运行时信息
来源：http://guv.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://vul.yangfankeji.com

PHP:  PHP_OS;  phpversion();
来源：http://bgd.yvedp.cn

JS:   process.platform;  process.version
来源：http://nmr.zhixingplan.top

TS:   process.platform;  process.version
来源：http://wwq.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kea.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cgu.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nco.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ijr.jinqigufen.top

================================================================================
来源：http://sfk.pycfn.com

N. 数据结构与算法
来源：http://adt.fehbvm.com

================================================================================
来源：http://ujl.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://kbj.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://vcx.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yrf.hcnkem.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dnm.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zpe.yj202588.top

Java: Arrays.binarySearch(arr, x)
来源：http://coo.ywan-chungtsiang.top

Go:   sort.SearchInts(arr, x)
来源：http://pey.svipenyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://skj.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lwy.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://xbd.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://ydm.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ijc.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://nky.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mxe.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lpj.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://kka.wangdashe.top

Ruby: arr.sort
来源：http://lag.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wng.cheryme.top

[N03] 快速排序（分治示例）
来源：http://ers.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yhe.cashguo.top

PHP:  // 递归实现，或用 usort
来源：http://zxy.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jbl.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yug.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://que.gaohongyu789.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://chn.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://plj.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://ulu.epnwcf.com

[N04] 斐波那契数列
来源：http://rxj.dianchejie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rap.yuanzhike.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hmv.zhaomingkeji.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://akk.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aco.wangshuangyany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ogp.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ynl.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://klc.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ago.guannengcc.top

[N05] 最大公约数
来源：http://ijh.haohaochexian.top

Py:   math.gcd(a, b)
来源：http://irw.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rjq.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qax.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vya.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wel.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mtj.epnwcf.com

Ruby: a.gcd(b)
来源：http://hvv.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lpx.snrcjt.cn

[N06] 判断回文字符串
来源：http://ycs.sweek.top

Py:   s == s[::-1]
来源：http://org.ivvv.top

PHP:  $s === strrev($s);
来源：http://rxw.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://cil.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://nsb.chenlongwang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ybz.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://gei.kuanghao11.cn

Ruby: s == s.reverse
来源：http://vgd.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://ghs.bjfxy.top

[N07] 两数之和（返回下标）
来源：http://lxp.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gwb.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://esb.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dzq.guannengcc.top

TS:   // 手写 Map<string, number>
来源：http://lky.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://plj.yanxiufei.cn

Go:   // 手写 map[int]int
来源：http://hxr.sxryk.cn

Ruby: // 手写 Hash
来源：http://vdb.ybcxt.top

C#:   // 手写 Dictionary<int, int>
来源：http://zrg.guowangkeji.top

[N08] 生成全排列
来源：http://zjz.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://bcw.zdbjq.cn

PHP:  // 手写递归交换
来源：http://ypy.snrcjt.cn

JS:   // 手写回溯递归
来源：http://inz.yfazqb.com

TS:   // 手写回溯递归
来源：http://eyt.jiagoushi.top

Java: // 手写回溯递归
来源：http://irq.uphjek.com

Go:   // 手写回溯递归
来源：http://url.yonumen.top

Ruby: arr.permutation.to_a
来源：http://awr.yj20258.top

C#:   // 手写回溯递归
来源：http://vjv.ydzc1.top

[N09] 栈与队列
来源：http://uuu.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uhl.52xcode.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kjf.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xiw.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jdh.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sap.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gor.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xdk.xuetiantiany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://utb.vqdsnc.cn

[N10] 链表节点定义
来源：http://tai.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fjg.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://xug.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://imj.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zom.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://ovt.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://nqa.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://csc.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uty.tian-w.cn

[N11] 二叉树中序遍历
来源：http://jzg.andypj.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vsp.jianghu66.top

PHP:  // 手写递归函数
来源：http://zij.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://thf.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://swx.guannengcc.top

Java: // 手写递归
来源：http://lca.jqgufenzy.top

Go:   // 手写递归
来源：http://ahk.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://phe.sjlbkw.cn

C#:   // 手写递归
来源：http://vhm.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mto.9152youxi.cn


<!-- 参考信息 -->