代发 wailian999

TS:   JSON.parse(s)
来源：http://oti.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://buy.aizwys.cn

Go:   json.Unmarshal(data, &v)
来源：http://jqm.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://stk.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qhl.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://yic.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mho.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vdr.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dew.shanyushiyangkeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://imn.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://okx.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gml.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://kof.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zic.iojbl.cn

[K04] 读取 JSON 文件
来源：http://wew.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wrh.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kku.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ger.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yvq.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lpg.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qaa.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://mvy.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mbs.9152youxi.cn

[K05] 深拷贝对象
来源：http://zck.zhixingplan.top

Py:   copy.deepcopy(obj)
来源：http://lxu.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://dkc.jiagoushi.top

JS:   structuredClone(obj)
来源：http://cfd.feifeiyinyue.top

TS:   structuredClone(obj)
来源：http://pau.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://epn.daxiang520.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ddh.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zfd.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://pil.daria6918.cn

[K06] 解析 URL 查询串
来源：http://pjs.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mpo.vqdsnc.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://giz.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nwr.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gkj.jianghu66.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://luj.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://imw.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zux.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kkh.yfazqb.com

[K07] 进制转换
来源：http://hfq.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://del.ppjwa.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lmv.tianlin.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://enz.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://whz.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pxl.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://agf.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cvg.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wta.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://hxq.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://qdr.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tym.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://egv.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://iaf.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kxu.yj202588.top

Go:   encoding/gob
来源：http://zoy.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://wvu.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cpw.zhongyouzk.top

================================================================================
来源：http://moa.nwbrower.top

L. 网络请求
来源：http://rfi.vqdsnc.cn

================================================================================
来源：http://gfi.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://wnm.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dqi.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ehx.cdnleiting.top

JS:   await fetch(url)
来源：http://xxj.ybcxt.top

TS:   await fetch(url)
来源：http://irn.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rdc.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://yhp.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pey.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zky.nanxinkj.top

[L02] 发送 POST JSON
来源：http://aul.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://jji.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xdi.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uep.sweek.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vlo.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sfy.yonumen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vle.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hvj.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iys.mhx1999.top

[L03] 设置自定义请求头
来源：http://xbb.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dcl.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bab.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://feb.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lhd.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tng.xziqi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mik.xingfuxueyuan.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lbm.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lnk.yuxming.cn

[L04] 设置超时
来源：http://ffz.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://zji.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fqh.pycfn.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gse.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ybn.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zmm.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ggi.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hvj.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ztt.ydjk.org.cn

[L05] 上传文件（multipart）
来源：http://yke.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jhu.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cdw.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mok.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://puy.jqgfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pbm.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fiz.yonumen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cmj.snrcjt.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://irw.cheryme.top

[L06] 解析响应为 JSON
来源：http://qdm.pengpengdd.cyou

Py:   resp.json()
来源：http://jfa.52xcode.cn

PHP:  json_decode($body, true);
来源：http://mpa.hongshengwenyu.top

JS:   await resp.json()
来源：http://uvz.tarul.cn

TS:   await resp.json()
来源：http://lwm.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rdf.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wtp.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://hyz.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lqf.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://yvg.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://khc.iojbl.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rhd.tarul.cn

JS:   resp.ok;  resp.status
来源：http://zqk.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://dsk.316326.xyz

Java: resp.statusCode()
来源：http://xnc.hesvh.cn

Go:   resp.StatusCode
来源：http://qss.andypj.xyz

Ruby: resp.code.to_i
来源：http://kin.shanyushiyangtech.top

C#:   (int)resp.StatusCode
来源：http://xmn.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://bgp.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vpm.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://tmg.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dhx.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ueu.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nok.tanke756.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cmt.fzhhl.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eya.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sli.havefunace.top

================================================================================
来源：http://kba.yangfankeji.com

M. 命令行 / 进程 / 环境
来源：http://qub.fzhhl.top

================================================================================
来源：http://tht.xylfe.cn

[M01] 读取命令行参数
来源：http://uyt.chenzaomai.com

Py:   sys.argv[1:]
来源：http://udb.xylfe.cn

PHP:  $argv;  $argc;
来源：http://ibb.hcnkem.com

JS:   process.argv.slice(2)
来源：http://skn.bjfxy.top

TS:   process.argv.slice(2)
来源：http://gqn.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://eha.tarul.cn

Go:   os.Args[1:]
来源：http://fia.pengpengdd.cyou

Ruby: ARGV
来源：http://gxr.nwbrower.top

C#:   args 数组（Main 方法参数）
来源：http://vmo.nanxuanxn.top

[M02] 读取环境变量
来源：http://vvt.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://oba.jlsjyb.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zvw.hammf.cn

JS:   process.env.HOME
来源：http://ueg.nwbrower.top

TS:   process.env.HOME
来源：http://geo.jinqigufen.top

Java: System.getenv("HOME")
来源：http://uyv.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vmh.gaohongyu789.top

Ruby: ENV["HOME"]
来源：http://hzz.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mrf.yuanzhike.top

[M03] 执行外部命令
来源：http://smg.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hkn.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://syt.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fzg.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vfy.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gqk.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ahk.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://owv.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://xwi.smart0.xyz

[M04] 获取当前工作目录
来源：http://dxn.hywenlv.cn

Py:   os.getcwd()
来源：http://vwp.hesvh.cn

PHP:  getcwd();
来源：http://tov.yangfankeji.com

JS:   process.cwd()
来源：http://dek.zhijiandao.cn

TS:   process.cwd()
来源：http://mde.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://qaw.hysaishi.cn

Go:   os.Getwd()
来源：http://gng.shuidangran.top

Ruby: Dir.pwd
来源：http://dcx.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://qiy.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://tdr.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://yec.zdqjudy.top

PHP:  exit(1);
来源：http://vlk.ivvv.top

JS:   process.exit(1)
来源：http://tla.cdnleiting.top

TS:   process.exit(1)
来源：http://muf.ivvv.top

Java: System.exit(1)
来源：http://jjo.52xcode.cn

Go:   os.Exit(1)
来源：http://prh.snrcjt.cn

Ruby: exit 1
来源：http://dng.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://emc.ybcxt.top

[M06] 向标准错误输出
来源：http://lms.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://ywk.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bxk.fengsongda.top

JS:   console.error("err")
来源：http://hsr.yangfankeji.com

TS:   console.error("err")
来源：http://auv.hnxiangtu.top

Java: System.err.println("err")
来源：http://eee.shanyushiyangtech.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qgs.52xcode.cn

Ruby: warn "err"
来源：http://fam.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://khp.c1oappe.top

[M07] 判断是否为主入口
来源：http://sxn.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://zvm.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ita.tian-w.cn

JS:   require.main === module
来源：http://kul.dianchejie.cn

TS:   require.main === module
来源：http://ped.xylfe.cn

Java: public static void main(String[] args)
来源：http://bvn.nanxuanxn.top

Go:   func main()
来源：http://xqu.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nvm.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://wvo.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://lhc.fanxiaobao.xyz

Py:   platform.system();  platform.python_version()
来源：http://eom.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://zuv.zdbjq.cn

JS:   process.platform;  process.version
来源：http://sbl.ivvv.top

TS:   process.platform;  process.version
来源：http://ivm.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tql.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://xic.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eqj.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wqd.pengpengdd.cyou

================================================================================
来源：http://xzn.yuanzhike.top

N. 数据结构与算法
来源：http://mkt.zycfv.cn

================================================================================
来源：http://nra.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://mbt.xingfuxueyuan.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://euj.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ycy.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cgo.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://syv.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://quo.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://kdi.shuidangran.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zvo.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://dki.chenjidiqi.icu

[N02] 排序（工程实践用内置实现）
来源：http://xen.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://bil.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tbk.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bye.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://llu.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zsl.yueranfly.top

Go:   slices.Sort(arr)
来源：http://ahk.yangfankeji.com

Ruby: arr.sort
来源：http://vtr.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vih.zhijiandao.cn

[N03] 快速排序（分治示例）
来源：http://miz.andypj.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kvh.ydzc1.top

PHP:  // 递归实现，或用 usort
来源：http://clw.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eqk.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://itd.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ksi.tanke756.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://odj.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eim.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://vum.redwolf501.top

[N04] 斐波那契数列
来源：http://vyi.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sgk.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fqn.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wbz.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ivb.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://llv.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mmk.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xgn.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hla.hywenlv.cn

[N05] 最大公约数
来源：http://oej.vehdjk.com

Py:   math.gcd(a, b)
来源：http://gjw.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ucz.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wvs.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pbh.xylfe.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mfe.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hqz.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://pmv.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wtq.jinqigfzy.top

[N06] 判断回文字符串
来源：http://aih.hammf.cn

Py:   s == s[::-1]
来源：http://akl.sysykeji.top

PHP:  $s === strrev($s);
来源：http://ejk.xziqi.cn

JS:   s === [...s].reverse().join("")
来源：http://ysa.redwolf501.top

TS:   s === [...s].reverse().join("")
来源：http://caw.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://znn.ybcxt.top

Go:   // 双指针从两端比较
来源：http://jyg.yuxming.cn

Ruby: s == s.reverse
来源：http://vcz.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://omc.dianchejie.cn

[N07] 两数之和（返回下标）
来源：http://nic.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ebl.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cfg.ywan-chungtsiang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cmq.zhaomingkeji.xyz

TS:   // 手写 Map<string, number>
来源：http://rvm.yj20258888.top

Java: // 手写 HashMap
来源：http://gxt.c1oappe.top

Go:   // 手写 map[int]int
来源：http://ili.ydzc1.top

Ruby: // 手写 Hash
来源：http://jbc.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://oub.meibo888.top

[N08] 生成全排列
来源：http://gei.sweek.top

Py:   itertools.permutations(arr)
来源：http://tvj.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://sde.birdmap.top

JS:   // 手写回溯递归
来源：http://gap.xingfuxueyuan.xyz

TS:   // 手写回溯递归
来源：http://ghh.ybcxt.top

Java: // 手写回溯递归
来源：http://zlq.snrcjt.cn

Go:   // 手写回溯递归
来源：http://fjd.sjlbkw.cn

Ruby: arr.permutation.to_a
来源：http://duh.uphjek.com

C#:   // 手写回溯递归
来源：http://bou.ydjk.org.cn

[N09] 栈与队列
来源：http://wwr.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rqj.hnxiangtu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uic.wangdashe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hej.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rrn.quarkkingdee.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xez.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gwm.hnxiangtu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dob.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jff.yj202588.top

[N10] 链表节点定义
来源：http://gkf.gzhubu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wef.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ciz.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xsa.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ruo.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://hbg.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hea.kuanghao11.cn


<!-- 参考信息 -->