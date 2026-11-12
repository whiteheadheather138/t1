代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://zeg.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gbs.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qzm.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vdf.sjlbkw.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tln.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hgx.aizwys.cn

[K04] 读取 JSON 文件
来源：http://scu.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://imb.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://afn.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vwa.ivvv.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eww.gotoacloud.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cuk.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zbl.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://cyq.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sgc.shuidangran.top

[K05] 深拷贝对象
来源：http://xdl.zhixingplan.top

Py:   copy.deepcopy(obj)
来源：http://mdd.zhijiandao.cn

PHP:  unserialize(serialize($obj));
来源：http://qbf.ivvv.top

JS:   structuredClone(obj)
来源：http://yba.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://nyz.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://egs.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zbt.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://edv.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://yrn.pengpengdd.cyou

[K06] 解析 URL 查询串
来源：http://sbt.shangyingyoupin.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ynl.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://byk.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kux.chenzaomai.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://smm.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://onq.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xlt.zhiwuduotai.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dtg.yueranfly.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wuh.jinqigfzy.top

[K07] 进制转换
来源：http://sde.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gvf.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://svw.iojbl.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kxp.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gjx.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lbx.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://glu.yvedp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dih.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zdi.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://lxc.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://lqe.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://jys.ydzc1.top

JS:   v8.serialize(obj)        // Node
来源：http://yga.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://ygd.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wcx.yuanzhike.top

Go:   encoding/gob
来源：http://woo.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://myu.vehdjk.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hws.jqgufenzy.top

================================================================================
来源：http://hqn.cdnleiting.top

L. 网络请求
来源：http://nsu.hfpthk.cn

================================================================================
来源：http://klz.hesvh.cn

[L01] 发送 GET 请求
来源：http://hnt.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sgh.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lya.jqgfzy.top

JS:   await fetch(url)
来源：http://wec.yangfankeji.com

TS:   await fetch(url)
来源：http://rdb.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vmz.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://kao.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://pmz.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xca.yj20258888.top

[L02] 发送 POST JSON
来源：http://iue.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://ybl.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lit.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zem.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hif.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tnp.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tye.yj20258888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pal.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gvg.jqgfzy.top

[L03] 设置自定义请求头
来源：http://haj.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://puc.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hwb.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nay.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://huu.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://usl.guowangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://brr.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sqe.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gxa.fengsongda.top

[L04] 设置超时
来源：http://emz.cucudq.cn

Py:   requests.get(url, timeout=5)
来源：http://rze.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mqs.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://miw.jinghuilouyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jvn.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://buh.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yth.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ltb.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cfo.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://dli.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ktc.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kpg.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bsp.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vkl.yuxming.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hiy.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xko.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gbm.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dve.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://mwo.cucudq.cn

Py:   resp.json()
来源：http://pgu.nwbrower.top

PHP:  json_decode($body, true);
来源：http://yqv.shangyingyoupin.top

JS:   await resp.json()
来源：http://ltw.tianlin.xyz

TS:   await resp.json()
来源：http://apl.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lhf.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pia.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://ljp.zdqjudy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cpt.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://pfe.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oof.andypj.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xkj.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://iki.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://esc.yfazqb.com

Java: resp.statusCode()
来源：http://fdu.aibaodan.cn

Go:   resp.StatusCode
来源：http://uph.xziqi.cn

Ruby: resp.code.to_i
来源：http://omq.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://ifb.316326.xyz

[L08] 并发请求多个地址
来源：http://qbm.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cvy.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://hjx.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eky.zdqjudy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hbv.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xjz.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cin.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cvw.birdmap.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wza.sysykeji.top

================================================================================
来源：http://jdi.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://zfp.yvedp.cn

================================================================================
来源：http://dql.hywenlv.cn

[M01] 读取命令行参数
来源：http://qpx.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://awc.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://elb.yj20258.top

JS:   process.argv.slice(2)
来源：http://kmg.yj202588.top

TS:   process.argv.slice(2)
来源：http://wgx.dianchejie.cn

Java: args 数组（main 方法参数）
来源：http://nxs.yj20258888.top

Go:   os.Args[1:]
来源：http://ghp.xziqi.cn

Ruby: ARGV
来源：http://zzg.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://bwv.dashuyun.cn

[M02] 读取环境变量
来源：http://cqq.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://uop.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gyn.pycfn.com

JS:   process.env.HOME
来源：http://woi.smart0.xyz

TS:   process.env.HOME
来源：http://yto.bjfxy.top

Java: System.getenv("HOME")
来源：http://shu.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oyd.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://sjt.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sbj.daxiang520.top

[M03] 执行外部命令
来源：http://isu.wangshuangyany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xlv.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iwb.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zsf.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://drl.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hwq.jinqigfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://baf.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tap.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://kvq.epnwcf.com

[M04] 获取当前工作目录
来源：http://asf.yonumen.top

Py:   os.getcwd()
来源：http://gml.yvedp.cn

PHP:  getcwd();
来源：http://dgk.hammf.cn

JS:   process.cwd()
来源：http://rjr.fengsongda.top

TS:   process.cwd()
来源：http://eqc.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://mul.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://yuk.jyoumei.cn

Ruby: Dir.pwd
来源：http://cie.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vbv.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://bkz.sweek.top

Py:   sys.exit(1)
来源：http://ljs.xuanzx.com

PHP:  exit(1);
来源：http://jlw.kuanghao11.cn

JS:   process.exit(1)
来源：http://cjq.tarul.cn

TS:   process.exit(1)
来源：http://oxc.jiagoushi.top

Java: System.exit(1)
来源：http://gaz.jinqigfzy.top

Go:   os.Exit(1)
来源：http://oca.zdqjudy.top

Ruby: exit 1
来源：http://iyw.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vfb.tarul.cn

[M06] 向标准错误输出
来源：http://xzp.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://jrb.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://tgk.jyoumei.cn

JS:   console.error("err")
来源：http://zvf.bbcook.cn

TS:   console.error("err")
来源：http://zeu.yvedp.cn

Java: System.err.println("err")
来源：http://lqo.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ktj.xylfe.cn

Ruby: warn "err"
来源：http://aux.c1oappe.top

C#:   Console.Error.WriteLine("err")
来源：http://cvx.hfpthk.cn

[M07] 判断是否为主入口
来源：http://ccw.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://hkt.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hmw.xylfe.cn

JS:   require.main === module
来源：http://ggr.chenlongwang.top

TS:   require.main === module
来源：http://eue.snrcjt.cn

Java: public static void main(String[] args)
来源：http://pgh.ppjwa.cn

Go:   func main()
来源：http://qcq.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dfu.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://ybw.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://vgg.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://vwe.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://ews.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://tlw.daxiang520.top

TS:   process.platform;  process.version
来源：http://zze.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qnb.xinyue.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://fux.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sby.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xxm.jinghuilouyu.cn

================================================================================
来源：http://tiw.cashguo.top

N. 数据结构与算法
来源：http://qwv.aizwys.cn

================================================================================
来源：http://qsm.tian-w.cn

[N01] 二分查找（有序数组）
来源：http://mxv.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pld.yuxming.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wdp.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ecp.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ssm.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://pmx.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://wws.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://twb.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hwm.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://zqs.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://mtv.hnxiangtu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fgg.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://nzn.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://piv.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ndw.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://jzy.dashuyun.cn

Ruby: arr.sort
来源：http://uaq.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ktx.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://nhy.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tpd.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://gki.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://msg.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fcd.yj20258.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wcy.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dcf.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bdv.shuidangran.top

C#:   // 手写递归，或 Array.Sort
来源：http://ntx.daxiang520.top

[N04] 斐波那契数列
来源：http://kjq.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bfx.yj20258.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ptq.fzhhl.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kmw.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dah.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xno.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zdk.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tfg.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jah.feifeiyinyue.top

[N05] 最大公约数
来源：http://jyk.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://vku.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lbw.zhengqikj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://asw.jyoumei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wtd.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pfe.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rwg.pengpengdd.cyou

Ruby: a.gcd(b)
来源：http://xsv.yj20258888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dnp.sysykeji.top

[N06] 判断回文字符串
来源：http://qpe.tanke756.top

Py:   s == s[::-1]
来源：http://bsq.daria6918.cn

PHP:  $s === strrev($s);
来源：http://eht.gaohongyu789.top

JS:   s === [...s].reverse().join("")
来源：http://jrl.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://ltm.hnxiangtu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wty.yj20258.top

Go:   // 双指针从两端比较
来源：http://ukr.daria6918.cn

Ruby: s == s.reverse
来源：http://pzi.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cuz.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://ozb.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kxg.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nfo.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://iht.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://agg.cheryme.top

Java: // 手写 HashMap
来源：http://qof.fzhhl.top

Go:   // 手写 map[int]int
来源：http://dfj.dashuyun.cn

Ruby: // 手写 Hash
来源：http://ezq.wangdashe.top

C#:   // 手写 Dictionary<int, int>
来源：http://tuq.yueranfly.top

[N08] 生成全排列
来源：http://lwu.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://nja.jqgfzy.top

PHP:  // 手写递归交换
来源：http://jvz.chenzaomai.com

JS:   // 手写回溯递归
来源：http://rty.dashuyun.cn

TS:   // 手写回溯递归
来源：http://zgp.gaohongyu789.top

Java: // 手写回溯递归
来源：http://lmy.chenzaomai.com

Go:   // 手写回溯递归
来源：http://ufo.zhoulong.xyz

Ruby: arr.permutation.to_a
来源：http://gdv.jlsjyb.cn

C#:   // 手写回溯递归
来源：http://wbg.andypj.xyz

[N09] 栈与队列
来源：http://oqo.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ubg.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mbj.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://osv.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cyn.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://edb.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aju.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kpb.nanxuanxn.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bal.sjlbkw.cn

[N10] 链表节点定义
来源：http://gns.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://usr.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ohy.daria6918.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://khd.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nja.bjfxy.top

Java: class Node { int v; Node next; }
来源：http://wxs.aibaodan.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dqs.shuidangran.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hgm.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://jmx.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://siu.hnqzz.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://azm.gotoacloud.top

PHP:  // 手写递归函数
来源：http://mqv.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ojn.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wvu.tian-w.cn

Java: // 手写递归
来源：http://hky.shzxlz.cn


<!-- 参考信息 -->