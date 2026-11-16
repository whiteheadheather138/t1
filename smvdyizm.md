代发 wailian999

TS:   JSON.parse(s)
来源：http://mwm.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vzf.fktsv.cn

Go:   json.Unmarshal(data, &v)
来源：http://isg.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://sfj.cheryme.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kwb.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://git.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hdf.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://idc.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://erw.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ytk.svipenyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xzg.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pux.jinqigufen.top

Ruby: JSON.pretty_generate(obj)
来源：http://fqi.nanxinkj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ecv.gzhubu.top

[K04] 读取 JSON 文件
来源：http://yzc.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lby.yueranfly.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hmr.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vin.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qvu.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://muq.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fow.ivvv.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zng.cheryme.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hlh.hammf.cn

[K05] 深拷贝对象
来源：http://brq.uphjek.com

Py:   copy.deepcopy(obj)
来源：http://med.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://dbl.feifeiyinyue.top

JS:   structuredClone(obj)
来源：http://nlw.tianlin.xyz

TS:   structuredClone(obj)
来源：http://jyx.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vpo.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cne.cqqwz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ptb.vqdsnc.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vrn.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://job.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ydj.gaohongyu789.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dtu.daria6918.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aja.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lye.tian-w.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bcl.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bcm.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hto.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kwr.cucudq.cn

[K07] 进制转换
来源：http://fsc.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xmz.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gcn.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rpd.haohaochexian.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rcv.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zbe.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rev.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uob.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rar.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://qfb.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://yyq.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ony.chenzaomai.com

JS:   v8.serialize(obj)        // Node
来源：http://ltq.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://tav.zycfv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gpa.cucudq.cn

Go:   encoding/gob
来源：http://bpw.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://kvw.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fqm.jinqigufen.top

================================================================================
来源：http://nuf.zhijiandao.cn

L. 网络请求
来源：http://mic.shzxlz.cn

================================================================================
来源：http://aus.chenjidiqi.icu

[L01] 发送 GET 请求
来源：http://sex.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pqf.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lkz.fehbvm.com

JS:   await fetch(url)
来源：http://zrt.meibo888.top

TS:   await fetch(url)
来源：http://rab.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bpq.zdqjudy.top

Go:   resp, err := http.Get(url)
来源：http://sge.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wyo.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ije.xylfe.cn

[L02] 发送 POST JSON
来源：http://shu.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://iir.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://paq.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rjn.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pyk.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://soe.fehbvm.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fed.cheryme.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wyd.jinghuilouyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uzh.jianghu66.top

[L03] 设置自定义请求头
来源：http://bse.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mup.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kqj.iojbl.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hmr.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jdt.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://acb.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dwj.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zif.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oqf.vqdsnc.cn

[L04] 设置超时
来源：http://evv.uphjek.com

Py:   requests.get(url, timeout=5)
来源：http://loy.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vkz.fktsv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wxg.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gyo.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kuz.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dne.jinqigfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dyf.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pze.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://cmz.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://quk.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bxq.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vhq.zhengqikj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cvf.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ldz.9152youxi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dwr.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vnb.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tdz.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://nxz.shanyushiyangkeji.top

Py:   resp.json()
来源：http://wzf.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://mkh.hesvh.cn

JS:   await resp.json()
来源：http://vga.wangdashe.top

TS:   await resp.json()
来源：http://oed.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uvf.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ahh.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://mxl.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gdr.uphjek.com

[L07] 处理 HTTP 状态码
来源：http://qcn.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rke.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://myq.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://zwr.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://gvd.9152youxi.cn

Java: resp.statusCode()
来源：http://gwj.tian-w.cn

Go:   resp.StatusCode
来源：http://hdp.nanxinkj.top

Ruby: resp.code.to_i
来源：http://pvw.daxiang520.top

C#:   (int)resp.StatusCode
来源：http://kav.havefunace.top

[L08] 并发请求多个地址
来源：http://eea.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tgl.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://trz.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ftn.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hck.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kkr.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uab.smart0.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://msu.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://emm.shzxlz.cn

================================================================================
来源：http://ftj.hfpthk.cn

M. 命令行 / 进程 / 环境
来源：http://hcj.sweek.top

================================================================================
来源：http://jxt.xziqi.cn

[M01] 读取命令行参数
来源：http://vqy.yangfankeji.com

Py:   sys.argv[1:]
来源：http://lrf.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://otk.xziqi.cn

JS:   process.argv.slice(2)
来源：http://bzp.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://ira.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://jsx.xingfuxueyuan.xyz

Go:   os.Args[1:]
来源：http://rtk.kuanghao11.cn

Ruby: ARGV
来源：http://llb.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://kkv.zhoulong.xyz

[M02] 读取环境变量
来源：http://nug.shuidangran.top

Py:   os.environ.get("HOME")
来源：http://age.aibaodan.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lyg.ivvv.top

JS:   process.env.HOME
来源：http://pyo.haohaochexian.top

TS:   process.env.HOME
来源：http://onp.aibaodan.cn

Java: System.getenv("HOME")
来源：http://jzj.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://usk.pycfn.com

Ruby: ENV["HOME"]
来源：http://vvs.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://icv.dianchejie.cn

[M03] 执行外部命令
来源：http://mte.zhongyouzk.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zyr.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xzo.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nso.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://xia.mhx1999.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://imc.mhx1999.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gvh.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://nui.zhoulong.xyz

C#:   Process.Start("ls", "-l");
来源：http://ubk.52xcode.cn

[M04] 获取当前工作目录
来源：http://pae.chenlongwang.top

Py:   os.getcwd()
来源：http://lyp.zhiwuduotai.top

PHP:  getcwd();
来源：http://roz.cucudq.cn

JS:   process.cwd()
来源：http://vrx.gogol.net.cn

TS:   process.cwd()
来源：http://nsz.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://ivk.hfpthk.cn

Go:   os.Getwd()
来源：http://ubg.xziqi.cn

Ruby: Dir.pwd
来源：http://gwx.jyoumei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://psh.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://jrh.zhengqikj.top

Py:   sys.exit(1)
来源：http://zfj.gaohongyu789.top

PHP:  exit(1);
来源：http://mwl.zhiwuduotai.top

JS:   process.exit(1)
来源：http://smy.yvedp.cn

TS:   process.exit(1)
来源：http://lmt.jyoumei.cn

Java: System.exit(1)
来源：http://thh.c1oappe.top

Go:   os.Exit(1)
来源：http://adg.tian-w.cn

Ruby: exit 1
来源：http://wyw.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zef.gogol.net.cn

[M06] 向标准错误输出
来源：http://hmz.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://kzg.jinyuanbaomall.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jqn.ctjpmb.com

JS:   console.error("err")
来源：http://flu.hesvh.cn

TS:   console.error("err")
来源：http://ney.fengsongda.top

Java: System.err.println("err")
来源：http://yqc.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://boj.fanxiaobao.xyz

Ruby: warn "err"
来源：http://pza.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://sjg.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://wsg.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://whk.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mct.cdnleiting.top

JS:   require.main === module
来源：http://vfr.fengsongda.top

TS:   require.main === module
来源：http://spq.birdmap.top

Java: public static void main(String[] args)
来源：http://vtp.chenlongwang.top

Go:   func main()
来源：http://zyh.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ekd.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://cow.snrcjt.cn

[M08] 获取系统与运行时信息
来源：http://aml.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://bes.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://qcl.hnqzz.top

JS:   process.platform;  process.version
来源：http://gay.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://gsx.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zwy.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ajy.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ski.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://lmf.quarkkingdee.top

================================================================================
来源：http://gpy.dashuyun.cn

N. 数据结构与算法
来源：http://vsf.hnqzz.top

================================================================================
来源：http://mnw.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://tfc.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://wmt.zhaomingkeji.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xwi.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sdn.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wtn.smart0.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://cii.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://cde.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qle.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://kpr.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://vef.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://nre.jlsjyb.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cgr.52xcode.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://egt.ybcxt.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ggf.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uij.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://mgx.shangyingyoupin.top

Ruby: arr.sort
来源：http://ptk.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yhn.52xcode.cn

[N03] 快速排序（分治示例）
来源：http://ukl.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ghf.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://kgu.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://klk.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://urc.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zam.dianchejie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vzq.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wdf.fzhhl.top

C#:   // 手写递归，或 Array.Sort
来源：http://rwd.havefunace.top

[N04] 斐波那契数列
来源：http://ibu.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zcc.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ztw.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tdl.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xxw.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bwz.hywenlv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://afl.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://van.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gcy.ybcxt.top

[N05] 最大公约数
来源：http://osu.cashguo.top

Py:   math.gcd(a, b)
来源：http://cgf.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rhy.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fok.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://igr.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xqn.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fop.wangdashe.top

Ruby: a.gcd(b)
来源：http://fvr.jlsjyb.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gie.cdnleiting.top

[N06] 判断回文字符串
来源：http://hug.yongpay.top

Py:   s == s[::-1]
来源：http://qlh.yvedp.cn

PHP:  $s === strrev($s);
来源：http://tep.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://peo.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://ute.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mib.yj20258888.top

Go:   // 双指针从两端比较
来源：http://zbu.daxiang520.top

Ruby: s == s.reverse
来源：http://fgr.hesvh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sak.zdbjq.cn

[N07] 两数之和（返回下标）
来源：http://aed.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://icf.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cdh.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yui.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://otf.shangyingyoupin.top

Java: // 手写 HashMap
来源：http://sby.smart0.xyz

Go:   // 手写 map[int]int
来源：http://cgr.guowangkeji.top

Ruby: // 手写 Hash
来源：http://xir.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zpt.wangshuangyany.cn

[N08] 生成全排列
来源：http://jgt.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://gto.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://rwe.yj202588.top

JS:   // 手写回溯递归
来源：http://yvl.fehbvm.com

TS:   // 手写回溯递归
来源：http://pxz.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://gbv.birdmap.top

Go:   // 手写回溯递归
来源：http://fkz.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://nyt.daria6918.cn

C#:   // 手写回溯递归
来源：http://yyi.sweek.top

[N09] 栈与队列
来源：http://frc.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://njr.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ney.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lwo.9152youxi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://txe.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bxb.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fqe.hammf.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ylo.xylfe.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ovz.cucudq.cn

[N10] 链表节点定义
来源：http://jkl.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://occ.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fhv.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cvf.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nzy.sweek.top

Java: class Node { int v; Node next; }
来源：http://rcu.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://jme.ehwqpu.com


<!-- 参考信息 -->