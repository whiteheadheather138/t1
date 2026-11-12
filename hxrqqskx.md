代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tsb.nanxuanxn.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://scz.ivvv.top

JS:   JSON.stringify(obj)
来源：http://yil.meibo888.top

TS:   JSON.stringify(obj)
来源：http://qgi.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ipg.ydzc1.top

Go:   json.Marshal(obj)
来源：http://qnh.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://rpq.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://who.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://vbr.c1oappe.top

Py:   json.loads(s)
来源：http://nid.shuidangran.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bvd.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://jsv.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://cwc.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://guh.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://atl.meibo888.top

Ruby: JSON.parse(s)
来源：http://flb.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ghq.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://crv.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rrp.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jkc.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://smt.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://iux.svipenyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zxa.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dol.dashuyun.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vcm.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hcc.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://tvn.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gjh.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tuv.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mqt.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nsw.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bpu.fehbvm.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hhq.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://jjx.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ewl.aibaodan.cn

[K05] 深拷贝对象
来源：http://irk.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://tbl.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://zot.zhongyouzk.top

JS:   structuredClone(obj)
来源：http://thb.jyoumei.cn

TS:   structuredClone(obj)
来源：http://srf.jqgfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://odt.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cue.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://arw.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ytr.fktsv.cn

[K06] 解析 URL 查询串
来源：http://pqo.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pqe.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://umv.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://buz.ehwqpu.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aos.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bew.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mya.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jka.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iuw.zdqjudy.top

[K07] 进制转换
来源：http://cdz.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fgo.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mgb.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tum.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://idc.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uzk.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tto.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lfb.xuetiantiany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xbc.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://jgz.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://kxo.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tfd.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://ump.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://jli.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yar.yanxiufei.cn

Go:   encoding/gob
来源：http://gvn.xingfuxueyuan.xyz

Ruby: Marshal.dump(obj)
来源：http://jma.xuanzx.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ndq.zycfv.cn

================================================================================
来源：http://muf.pycfn.com

L. 网络请求
来源：http://ykp.yj20258888.top

================================================================================
来源：http://tyx.chenzaomai.com

[L01] 发送 GET 请求
来源：http://ssr.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rsn.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nyk.quarkkingdee.top

JS:   await fetch(url)
来源：http://twj.chenlongwang.top

TS:   await fetch(url)
来源：http://lwg.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://suf.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://xwq.vehdjk.com

Ruby: Net::HTTP.get(URI(url))
来源：http://dcn.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cxa.jqgfzy.top

[L02] 发送 POST JSON
来源：http://nwj.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://rno.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ate.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jvf.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oml.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://udl.bjfxy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pnl.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lci.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wix.bjfxy.top

[L03] 设置自定义请求头
来源：http://yle.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uum.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tuo.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fll.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kit.ivvv.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tfv.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vcm.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wge.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hdc.cheryme.top

[L04] 设置超时
来源：http://dcm.sweek.top

Py:   requests.get(url, timeout=5)
来源：http://nyy.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hhg.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qal.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wkk.zhaomingkeji.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ixk.hywenlv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dug.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pza.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://orm.xziqi.cn

[L05] 上传文件（multipart）
来源：http://mth.zycfv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gbx.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qud.fengsongda.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mco.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mea.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eng.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://njd.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wec.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ylj.shuidangran.top

[L06] 解析响应为 JSON
来源：http://miy.yanxiufei.cn

Py:   resp.json()
来源：http://vya.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://vuu.hfpthk.cn

JS:   await resp.json()
来源：http://ega.hongshengwenyu.top

TS:   await resp.json()
来源：http://lqt.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fzp.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xis.chenjidiqi.icu

Ruby: JSON.parse(resp.body)
来源：http://wlp.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ovf.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://zfa.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sjj.hnqzz.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jxb.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://dub.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://mie.shangyingyoupin.top

Java: resp.statusCode()
来源：http://lom.daria6918.cn

Go:   resp.StatusCode
来源：http://soe.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://bnw.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://ale.iojbl.cn

[L08] 并发请求多个地址
来源：http://phw.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zwq.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://wik.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kwk.xziqi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fjs.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vjm.shangyingyoupin.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wuj.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ojj.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uxh.iojbl.cn

================================================================================
来源：http://kxa.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://qpc.epnwcf.com

================================================================================
来源：http://ztv.ctjpmb.com

[M01] 读取命令行参数
来源：http://fed.yj20258.top

Py:   sys.argv[1:]
来源：http://dqu.jlsjyb.cn

PHP:  $argv;  $argc;
来源：http://lkx.fktsv.cn

JS:   process.argv.slice(2)
来源：http://rxs.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://zko.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://jto.vehdjk.com

Go:   os.Args[1:]
来源：http://lhe.yangfankeji.com

Ruby: ARGV
来源：http://iap.zhengqikj.top

C#:   args 数组（Main 方法参数）
来源：http://hhp.fengsongda.top

[M02] 读取环境变量
来源：http://hoj.gotoacloud.top

Py:   os.environ.get("HOME")
来源：http://ake.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mfx.sxryk.cn

JS:   process.env.HOME
来源：http://fmn.hammf.cn

TS:   process.env.HOME
来源：http://vjz.uphjek.com

Java: System.getenv("HOME")
来源：http://zit.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ppk.sysykeji.top

Ruby: ENV["HOME"]
来源：http://fio.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nie.ctjpmb.com

[M03] 执行外部命令
来源：http://aoh.ehwqpu.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bqv.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bup.hnxiangtu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://abu.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fbj.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ojy.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wih.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yju.zhaomingkeji.xyz

C#:   Process.Start("ls", "-l");
来源：http://jwp.xinyue.icu

[M04] 获取当前工作目录
来源：http://oqp.shzxlz.cn

Py:   os.getcwd()
来源：http://eim.aibaodan.cn

PHP:  getcwd();
来源：http://drz.nwbrower.top

JS:   process.cwd()
来源：http://uyb.smart0.xyz

TS:   process.cwd()
来源：http://zet.uphjek.com

Java: Path.of("").toAbsolutePath()
来源：http://xbm.cheryme.top

Go:   os.Getwd()
来源：http://une.c1oappe.top

Ruby: Dir.pwd
来源：http://pej.9152youxi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://war.ivvv.top

[M05] 设置退出码
来源：http://xdi.vehdjk.com

Py:   sys.exit(1)
来源：http://mcs.meibo888.top

PHP:  exit(1);
来源：http://cyz.yj20258.top

JS:   process.exit(1)
来源：http://hqb.chenlongwang.top

TS:   process.exit(1)
来源：http://zau.haohaochexian.top

Java: System.exit(1)
来源：http://tij.ctjpmb.com

Go:   os.Exit(1)
来源：http://mcy.xuetiantiany.cn

Ruby: exit 1
来源：http://mjt.smart0.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ita.nanxinkj.top

[M06] 向标准错误输出
来源：http://kek.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://alz.cashguo.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vwp.cheryme.top

JS:   console.error("err")
来源：http://tis.dianchejie.cn

TS:   console.error("err")
来源：http://ijg.gaohongyu789.top

Java: System.err.println("err")
来源：http://usn.gogol.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qsi.daxiang520.top

Ruby: warn "err"
来源：http://vvn.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://sdx.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://dvs.cheryme.top

Py:   if __name__ == "__main__":
来源：http://rdd.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vzj.sweek.top

JS:   require.main === module
来源：http://ikl.shanyushiyangkeji.top

TS:   require.main === module
来源：http://bsm.jiagoushi.top

Java: public static void main(String[] args)
来源：http://som.shanyushiyangkeji.top

Go:   func main()
来源：http://lva.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hvp.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://zng.jqgfzy.top

[M08] 获取系统与运行时信息
来源：http://oxe.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://upk.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://zbb.wangdashe.top

JS:   process.platform;  process.version
来源：http://cme.52xcode.cn

TS:   process.platform;  process.version
来源：http://xjn.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jjr.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ria.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mvu.havefunace.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zju.zdbjq.cn

================================================================================
来源：http://mdb.hongshengwenyu.top

N. 数据结构与算法
来源：http://hdz.tian-w.cn

================================================================================
来源：http://ztk.yongpay.top

[N01] 二分查找（有序数组）
来源：http://fsa.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rgt.zhoulong.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vhk.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://prt.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dax.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://gdn.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://lwy.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jdj.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://pvi.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://fto.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://fpi.jinqigufen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://usk.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://dhb.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xva.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mmi.316326.xyz

Go:   slices.Sort(arr)
来源：http://mxb.sysykeji.top

Ruby: arr.sort
来源：http://zbd.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xni.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://zsy.zhoulong.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eab.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://dam.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gre.vqdsnc.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jlz.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nxi.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vzz.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iec.zhongyouzk.top

C#:   // 手写递归，或 Array.Sort
来源：http://wqi.snrcjt.cn

[N04] 斐波那契数列
来源：http://pgf.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://omz.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bpq.meibo888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rxq.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pfk.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uti.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://afw.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ozf.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://soa.sjlbkw.cn

[N05] 最大公约数
来源：http://lef.zdqjudy.top

Py:   math.gcd(a, b)
来源：http://lvs.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xfw.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iub.yfazqb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kww.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lce.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cwu.redwolf501.top

Ruby: a.gcd(b)
来源：http://xlv.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ani.jinqigfzy.top

[N06] 判断回文字符串
来源：http://qnm.smart0.xyz

Py:   s == s[::-1]
来源：http://ves.tarul.cn

PHP:  $s === strrev($s);
来源：http://uqn.gzhubu.top

JS:   s === [...s].reverse().join("")
来源：http://ych.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://drf.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wzc.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://dzq.yj20258888.top

Ruby: s == s.reverse
来源：http://ewc.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://aqp.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://uzh.ivvv.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://guz.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lis.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tdg.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://lxw.bjfxy.top

Java: // 手写 HashMap
来源：http://tme.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://pcx.52xcode.cn

Ruby: // 手写 Hash
来源：http://qeq.316326.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://nsl.tarul.cn

[N08] 生成全排列
来源：http://wiw.chenlongwang.top

Py:   itertools.permutations(arr)
来源：http://tmz.havefunace.top

PHP:  // 手写递归交换
来源：http://jve.yfazqb.com

JS:   // 手写回溯递归
来源：http://wfz.yj20258888.top

TS:   // 手写回溯递归
来源：http://vpg.jiagoushi.top

Java: // 手写回溯递归
来源：http://siv.cqqwz.cn

Go:   // 手写回溯递归
来源：http://oxw.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://lip.yangfankeji.com

C#:   // 手写回溯递归
来源：http://mnp.jianghu66.top

[N09] 栈与队列
来源：http://zcj.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vpa.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vhq.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ckf.pengpengdd.cyou


<!-- 参考信息 -->