代发 wailian999

[K02] JSON 字符串转对象
来源：http://wgb.xuanzx.com

Py:   json.loads(s)
来源：http://ysc.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ddl.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://abh.fehbvm.com

TS:   JSON.parse(s)
来源：http://cnp.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kct.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://mcv.zycfv.cn

Ruby: JSON.parse(s)
来源：http://itp.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ham.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://lqn.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fyh.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zjo.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bfj.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qov.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xdf.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zof.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://icg.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ldj.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://tfv.zdqjudy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xrq.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jcn.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lml.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kuf.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ter.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wqn.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://whs.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://was.uphjek.com

[K05] 深拷贝对象
来源：http://yqv.sweek.top

Py:   copy.deepcopy(obj)
来源：http://mqd.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://cmg.c1oappe.top

JS:   structuredClone(obj)
来源：http://qgj.cashguo.top

TS:   structuredClone(obj)
来源：http://yed.redwolf501.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yjn.hnqzz.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zqv.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gef.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://klu.fehbvm.com

[K06] 解析 URL 查询串
来源：http://xlv.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sec.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tdi.xuanzx.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oej.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vgs.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://enr.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://wfj.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xtj.jiagoushi.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://szf.wangshuangyany.cn

[K07] 进制转换
来源：http://jyc.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dee.xingfuxueyuan.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kwx.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wrt.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ypi.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://afl.316326.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eij.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xya.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kxy.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://bwy.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://cbv.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lvd.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://jgu.ydjk.org.cn

TS:   v8.serialize(obj)        // Node
来源：http://kef.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mfe.yangfankeji.com

Go:   encoding/gob
来源：http://tik.tarul.cn

Ruby: Marshal.dump(obj)
来源：http://mzr.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dsw.zhixingplan.top

================================================================================
来源：http://gzd.ywan-chungtsiang.top

L. 网络请求
来源：http://tpd.ehwqpu.com

================================================================================
来源：http://wro.daria6918.cn

[L01] 发送 GET 请求
来源：http://bky.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yck.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://apj.bjfxy.top

JS:   await fetch(url)
来源：http://ggz.cucudq.cn

TS:   await fetch(url)
来源：http://wyk.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://adb.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://vub.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hev.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ttx.nanxinkj.top

[L02] 发送 POST JSON
来源：http://hxn.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://elf.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jrx.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lqz.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lgk.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ufk.dianchejie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kdh.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hzy.yueranfly.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iwn.wangshuangyany.cn

[L03] 设置自定义请求头
来源：http://mhr.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lyt.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ihl.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rsa.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ygy.uphjek.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ixm.fehbvm.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kkl.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jbc.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dkq.aibaodan.cn

[L04] 设置超时
来源：http://cps.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://nrk.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cmk.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sfj.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pas.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://soy.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xvb.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kkj.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kxp.ivvv.top

[L05] 上传文件（multipart）
来源：http://kyo.wangdashe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://voq.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fbo.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gxm.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ltl.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fbq.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://plx.cdnleiting.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vsb.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uea.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://mjb.sufxvd.cn

Py:   resp.json()
来源：http://cdg.yongpay.top

PHP:  json_decode($body, true);
来源：http://jxq.xylfe.cn

JS:   await resp.json()
来源：http://shz.fzhhl.top

TS:   await resp.json()
来源：http://lqu.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uma.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://avy.xingfuxueyuan.xyz

Ruby: JSON.parse(resp.body)
来源：http://abh.tian-w.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fka.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://wfw.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wzd.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qtp.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://tpp.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://wmo.gotoacloud.top

Java: resp.statusCode()
来源：http://rqd.chenlongwang.top

Go:   resp.StatusCode
来源：http://zfq.yangfankeji.com

Ruby: resp.code.to_i
来源：http://xzr.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://nfp.jyoumei.cn

[L08] 并发请求多个地址
来源：http://wei.yfazqb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qob.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://lgo.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dvi.fktsv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bxj.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pre.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hbw.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sye.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qys.yfazqb.com

================================================================================
来源：http://sff.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://reh.jianghu66.top

================================================================================
来源：http://oix.cqqwz.cn

[M01] 读取命令行参数
来源：http://jms.pycfn.com

Py:   sys.argv[1:]
来源：http://jho.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://kug.birdmap.top

JS:   process.argv.slice(2)
来源：http://pts.yj20258.top

TS:   process.argv.slice(2)
来源：http://oec.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://ryz.snrcjt.cn

Go:   os.Args[1:]
来源：http://web.jianghu66.top

Ruby: ARGV
来源：http://hqw.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://kvu.sweek.top

[M02] 读取环境变量
来源：http://syc.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://dts.xziqi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mhk.bbcook.cn

JS:   process.env.HOME
来源：http://jnb.zdqjudy.top

TS:   process.env.HOME
来源：http://ukl.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://van.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://prd.andypj.xyz

Ruby: ENV["HOME"]
来源：http://mtv.fanxiaobao.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zxq.cqqwz.cn

[M03] 执行外部命令
来源：http://pxj.shangyingyoupin.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lvv.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://viz.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yem.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qmi.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ipu.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://tmm.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://suw.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://gmz.sysykeji.top

[M04] 获取当前工作目录
来源：http://plr.nanxuanxn.top

Py:   os.getcwd()
来源：http://ghf.daxiang520.top

PHP:  getcwd();
来源：http://fbf.mhx1999.top

JS:   process.cwd()
来源：http://rmd.hongshengwenyu.top

TS:   process.cwd()
来源：http://wuu.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://vss.hesvh.cn

Go:   os.Getwd()
来源：http://rtl.yj202588.top

Ruby: Dir.pwd
来源：http://gqf.jianghu66.top

C#:   Directory.GetCurrentDirectory()
来源：http://kpj.sysykeji.top

[M05] 设置退出码
来源：http://zxs.hysaishi.cn

Py:   sys.exit(1)
来源：http://kjg.hammf.cn

PHP:  exit(1);
来源：http://zfe.wangdashe.top

JS:   process.exit(1)
来源：http://hly.bbcook.cn

TS:   process.exit(1)
来源：http://kos.chenlongwang.top

Java: System.exit(1)
来源：http://fbe.sxryk.cn

Go:   os.Exit(1)
来源：http://wnl.yj20258.top

Ruby: exit 1
来源：http://abc.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kdj.svipenyu.cn

[M06] 向标准错误输出
来源：http://svq.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://nvh.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://omr.fehbvm.com

JS:   console.error("err")
来源：http://wvu.fehbvm.com

TS:   console.error("err")
来源：http://rxx.nanxuanxn.top

Java: System.err.println("err")
来源：http://uuf.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gwf.gotoacloud.top

Ruby: warn "err"
来源：http://qpe.uphjek.com

C#:   Console.Error.WriteLine("err")
来源：http://rsb.yuanzhike.top

[M07] 判断是否为主入口
来源：http://iit.dianchejie.cn

Py:   if __name__ == "__main__":
来源：http://gyk.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tjl.fengsongda.top

JS:   require.main === module
来源：http://bze.ydjk.org.cn

TS:   require.main === module
来源：http://iaa.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://wzr.shuidangran.top

Go:   func main()
来源：http://jnw.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qej.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://bmf.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://ckq.gogol.net.cn

Py:   platform.system();  platform.python_version()
来源：http://mhi.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://qnw.jyoumei.cn

JS:   process.platform;  process.version
来源：http://oao.ehwqpu.com

TS:   process.platform;  process.version
来源：http://gcc.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://emj.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://yza.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mya.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://voz.zhengqikj.top

================================================================================
来源：http://hic.nanxuanxn.top

N. 数据结构与算法
来源：http://soz.zhiwuduotai.top

================================================================================
来源：http://xec.uphjek.com

[N01] 二分查找（有序数组）
来源：http://gic.nwbrower.top

Py:   bisect.bisect_left(arr, x)
来源：http://lim.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aux.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nml.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zji.jinqigufen.top

Java: Arrays.binarySearch(arr, x)
来源：http://mmh.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://bsq.yj20258.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mnl.gzhubu.top

C#:   Array.BinarySearch(arr, x)
来源：http://vfu.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://abx.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://lle.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rgc.yonumen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://frg.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://tqx.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bdf.cashguo.top

Go:   slices.Sort(arr)
来源：http://zie.sufxvd.cn

Ruby: arr.sort
来源：http://lhd.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wqz.yj202588.top

[N03] 快速排序（分治示例）
来源：http://pms.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mts.zhaomingkeji.xyz

PHP:  // 递归实现，或用 usort
来源：http://wcx.ybcxt.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mfo.ppjwa.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wut.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jxj.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hff.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hzk.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://hwz.tian-w.cn

[N04] 斐波那契数列
来源：http://prx.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ssf.yfazqb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rms.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lxo.bjfxy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dfx.havefunace.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rfu.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lvz.hammf.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hmz.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://esj.xinyue.icu

[N05] 最大公约数
来源：http://jxp.iojbl.cn

Py:   math.gcd(a, b)
来源：http://jrq.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nal.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wqk.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ywg.yonumen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jao.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nde.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://ytq.hcnkem.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ayt.fengsongda.top

[N06] 判断回文字符串
来源：http://bue.tarul.cn

Py:   s == s[::-1]
来源：http://jpx.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://ggo.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://osx.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://oqe.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gww.cheryme.top

Go:   // 双指针从两端比较
来源：http://xbm.shuidangran.top

Ruby: s == s.reverse
来源：http://lvp.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xco.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://cil.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kwx.chenzaomai.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://alk.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pfz.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://mwp.0kj1m.cn

Java: // 手写 HashMap
来源：http://zqd.tanke756.top

Go:   // 手写 map[int]int
来源：http://sav.tianlin.xyz

Ruby: // 手写 Hash
来源：http://egn.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://cuk.yanxiufei.cn

[N08] 生成全排列
来源：http://mle.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://wzb.yuxming.cn

PHP:  // 手写递归交换
来源：http://xqg.yueranfly.top

JS:   // 手写回溯递归
来源：http://zzz.dianchejie.cn

TS:   // 手写回溯递归
来源：http://vwl.chenjidiqi.icu

Java: // 手写回溯递归
来源：http://qix.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://wfl.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://qwo.smart0.xyz

C#:   // 手写回溯递归
来源：http://lrx.yvedp.cn

[N09] 栈与队列
来源：http://jnt.shangyingyoupin.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ozx.52xcode.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gni.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lqa.xylfe.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tvi.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hve.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://our.jinqigfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://scg.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oxt.birdmap.top

[N10] 链表节点定义
来源：http://xwf.feifeiyinyue.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dpt.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nfj.shuidangran.top


<!-- 参考信息 -->