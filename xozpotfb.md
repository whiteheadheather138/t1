代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vre.jqgfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gby.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://avx.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wut.zdqjudy.top

================================================================================
来源：http://ylo.0kj1m.cn

K. JSON 与序列化
来源：http://ulq.wangdashe.top

================================================================================
来源：http://jdq.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://lxf.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ugr.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jiq.shangyingyoupin.top

JS:   JSON.stringify(obj)
来源：http://zfd.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://plz.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oma.epnwcf.com

Go:   json.Marshal(obj)
来源：http://rsz.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://nnb.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://xcz.tarul.cn

[K02] JSON 字符串转对象
来源：http://rqw.meibo888.top

Py:   json.loads(s)
来源：http://lel.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://opk.hywenlv.cn

JS:   JSON.parse(s)
来源：http://epw.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://yjl.yangfankeji.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aoi.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://wfg.c1oappe.top

Ruby: JSON.parse(s)
来源：http://hvm.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jlo.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://ife.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ccd.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://klx.hnxiangtu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hyz.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nce.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mro.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ran.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://blh.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rdb.xuanzx.com

[K04] 读取 JSON 文件
来源：http://fag.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zyz.havefunace.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uai.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wpo.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zwh.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://okc.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kav.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gvt.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pom.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://mzn.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://ryn.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://byq.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://ojs.aizwys.cn

TS:   structuredClone(obj)
来源：http://kdc.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hpy.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zyj.jqgfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jzo.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://iqa.yj202588.top

[K06] 解析 URL 查询串
来源：http://gvd.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://siw.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pfn.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gnx.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mlf.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pbk.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fwn.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yna.hammf.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mcm.tian-w.cn

[K07] 进制转换
来源：http://uir.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cma.gzhubu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vgb.ehwqpu.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nnj.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://efy.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ojj.ppjwa.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://meb.gzhubu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dks.ydzc1.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jdr.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://mlo.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://kkh.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://apc.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://zzw.ctjpmb.com

TS:   v8.serialize(obj)        // Node
来源：http://qiv.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tlq.xinyue.icu

Go:   encoding/gob
来源：http://bvu.gotoacloud.top

Ruby: Marshal.dump(obj)
来源：http://uzr.yj20258.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dgc.xingfuxueyuan.xyz

================================================================================
来源：http://uvl.shangyingyoupin.top

L. 网络请求
来源：http://nza.gaohongyu789.top

================================================================================
来源：http://prz.yj202588.top

[L01] 发送 GET 请求
来源：http://khj.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gqg.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ksn.jinghuilouyu.cn

JS:   await fetch(url)
来源：http://cqw.epnwcf.com

TS:   await fetch(url)
来源：http://fzv.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jfv.xziqi.cn

Go:   resp, err := http.Get(url)
来源：http://akp.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mer.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fqs.xuanzx.com

[L02] 发送 POST JSON
来源：http://rag.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dmy.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gbr.fengsongda.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kjn.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yha.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ooj.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eze.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fmd.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eqb.gzhubu.top

[L03] 设置自定义请求头
来源：http://jfg.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lcv.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tmu.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ead.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dxh.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ilr.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fsp.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mrn.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://isn.kuanghao11.cn

[L04] 设置超时
来源：http://txs.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://mni.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zgu.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://chi.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qhc.nanxinkj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rnz.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xdi.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://icq.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vak.guannengcc.top

[L05] 上传文件（multipart）
来源：http://szx.yj20258888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fxn.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://llc.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mhx.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://urj.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tev.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ycp.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jpe.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mml.zdqjudy.top

[L06] 解析响应为 JSON
来源：http://zfv.cdnleiting.top

Py:   resp.json()
来源：http://uds.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://uvc.zhiwuduotai.top

JS:   await resp.json()
来源：http://gga.ctjpmb.com

TS:   await resp.json()
来源：http://kle.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hpa.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://krc.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://xyo.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gex.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://yjk.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://udf.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eav.redwolf501.top

JS:   resp.ok;  resp.status
来源：http://cnf.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://mhp.gaohongyu789.top

Java: resp.statusCode()
来源：http://smd.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://bpe.zdbjq.cn

Ruby: resp.code.to_i
来源：http://sao.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://hct.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://nxv.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wzc.xinyue.icu

PHP:  curl_multi_init() 系列
来源：http://cvm.andypj.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sgw.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cvx.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xob.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uqw.zhengqikj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://per.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zvv.dashuyun.cn

================================================================================
来源：http://gpd.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://qsp.hfpthk.cn

================================================================================
来源：http://fss.ydzc1.top

[M01] 读取命令行参数
来源：http://jxn.vehdjk.com

Py:   sys.argv[1:]
来源：http://lwb.haohaochexian.top

PHP:  $argv;  $argc;
来源：http://ltx.iojbl.cn

JS:   process.argv.slice(2)
来源：http://law.xuetiantiany.cn

TS:   process.argv.slice(2)
来源：http://ynr.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://qhi.zhixingplan.top

Go:   os.Args[1:]
来源：http://vox.yj20258.top

Ruby: ARGV
来源：http://mmc.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://jny.chenlongwang.top

[M02] 读取环境变量
来源：http://xqj.hywenlv.cn

Py:   os.environ.get("HOME")
来源：http://gbr.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nrd.guowangkeji.top

JS:   process.env.HOME
来源：http://yat.sxryk.cn

TS:   process.env.HOME
来源：http://ymw.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://taf.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gdz.yongpay.top

Ruby: ENV["HOME"]
来源：http://kyw.cheryme.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tuq.fehbvm.com

[M03] 执行外部命令
来源：http://luy.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wtr.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oke.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wdo.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://boy.hesvh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cow.tarul.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xlr.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ywq.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://gwa.tian-w.cn

[M04] 获取当前工作目录
来源：http://aef.jyoumei.cn

Py:   os.getcwd()
来源：http://uic.chenjidiqi.icu

PHP:  getcwd();
来源：http://dqt.yanxiufei.cn

JS:   process.cwd()
来源：http://oov.redwolf501.top

TS:   process.cwd()
来源：http://miz.mhx1999.top

Java: Path.of("").toAbsolutePath()
来源：http://ggh.cucudq.cn

Go:   os.Getwd()
来源：http://nev.smart0.xyz

Ruby: Dir.pwd
来源：http://prj.zhengqikj.top

C#:   Directory.GetCurrentDirectory()
来源：http://fdy.cqqwz.cn

[M05] 设置退出码
来源：http://dnf.ydjk.org.cn

Py:   sys.exit(1)
来源：http://pki.uphjek.com

PHP:  exit(1);
来源：http://rjp.cashguo.top

JS:   process.exit(1)
来源：http://hkz.yuanzhike.top

TS:   process.exit(1)
来源：http://lzo.xuanzx.com

Java: System.exit(1)
来源：http://pbb.zdbjq.cn

Go:   os.Exit(1)
来源：http://qvj.jyoumei.cn

Ruby: exit 1
来源：http://kcc.zhijiandao.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yry.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://gwo.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://mbi.fktsv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jvi.zdqjudy.top

JS:   console.error("err")
来源：http://ahc.bjfxy.top

TS:   console.error("err")
来源：http://kja.316326.xyz

Java: System.err.println("err")
来源：http://djz.shanyushiyangtech.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://avj.yueranfly.top

Ruby: warn "err"
来源：http://dha.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://gwq.zhongyouzk.top

[M07] 判断是否为主入口
来源：http://hxl.jinqigufen.top

Py:   if __name__ == "__main__":
来源：http://jrg.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tok.uphjek.com

JS:   require.main === module
来源：http://ypm.fktsv.cn

TS:   require.main === module
来源：http://ulg.smart0.xyz

Java: public static void main(String[] args)
来源：http://yjl.9152youxi.cn

Go:   func main()
来源：http://beq.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://njq.yj20258888.top

C#:   static void Main(string[] args)
来源：http://gme.cheryme.top

[M08] 获取系统与运行时信息
来源：http://pia.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://uea.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://byg.nanxinkj.top

JS:   process.platform;  process.version
来源：http://tie.shzxlz.cn

TS:   process.platform;  process.version
来源：http://yxe.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qkx.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fvm.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tqw.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://lix.xingfuxueyuan.xyz

================================================================================
来源：http://wvm.svipenyu.cn

N. 数据结构与算法
来源：http://phm.0kj1m.cn

================================================================================
来源：http://hxe.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://zzk.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://toq.jianghu66.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tli.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ees.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qvy.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://myb.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://usg.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yqs.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://onr.hnxiangtu.top

[N02] 排序（工程实践用内置实现）
来源：http://snt.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://olf.uphjek.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xua.jyoumei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://osi.cqqwz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gpv.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pdy.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://yxu.chenjidiqi.icu

Ruby: arr.sort
来源：http://kkz.svipenyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jpr.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://xet.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://loy.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://dxg.svipenyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uhs.jqgfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qiu.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://avv.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xau.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bcb.yfazqb.com

C#:   // 手写递归，或 Array.Sort
来源：http://lyr.ehwqpu.com

[N04] 斐波那契数列
来源：http://vvu.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jcl.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kld.wangshuangyany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jcv.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://trf.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yhj.ydzc1.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xvc.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mhe.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ixp.0kj1m.cn

[N05] 最大公约数
来源：http://mui.epnwcf.com

Py:   math.gcd(a, b)
来源：http://coq.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wum.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mox.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uhg.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://epk.shangyingyoupin.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://spe.chenzaomai.com

Ruby: a.gcd(b)
来源：http://akt.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bea.xylfe.cn

[N06] 判断回文字符串
来源：http://nol.xylfe.cn

Py:   s == s[::-1]
来源：http://lqr.gzhubu.top

PHP:  $s === strrev($s);
来源：http://qmx.zdqjudy.top

JS:   s === [...s].reverse().join("")
来源：http://enl.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://ezc.sweek.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://idm.yonumen.top

Go:   // 双指针从两端比较
来源：http://cqe.hnqzz.top

Ruby: s == s.reverse
来源：http://jva.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jcc.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://cgv.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wzt.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://efa.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cyy.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://gho.daria6918.cn

Java: // 手写 HashMap
来源：http://xgr.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://tdl.chenlongwang.top

Ruby: // 手写 Hash
来源：http://guw.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://xjf.gaohongyu789.top

[N08] 生成全排列
来源：http://uos.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://kra.yj20258.top

PHP:  // 手写递归交换
来源：http://hls.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://bpu.birdmap.top

TS:   // 手写回溯递归
来源：http://osc.xziqi.cn


<!-- 参考信息 -->