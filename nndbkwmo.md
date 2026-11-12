代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uab.jianghu66.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qyq.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gzw.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://esa.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tvb.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lzr.xuetiantiany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bhu.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bzt.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ytx.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fkr.xziqi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://onc.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jtx.cucudq.cn

================================================================================
来源：http://ofc.cashguo.top

K. JSON 与序列化
来源：http://fui.fktsv.cn

================================================================================
来源：http://sdq.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://wnp.pengpengdd.cyou

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cfm.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nvi.316326.xyz

JS:   JSON.stringify(obj)
来源：http://yxx.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://nnq.fehbvm.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rdj.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://nqp.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://vta.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://soj.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://iae.guowangkeji.top

Py:   json.loads(s)
来源：http://rps.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bqs.shzxlz.cn

JS:   JSON.parse(s)
来源：http://yrp.shangyingyoupin.top

TS:   JSON.parse(s)
来源：http://gll.gotoacloud.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tjc.xuanzx.com

Go:   json.Unmarshal(data, &v)
来源：http://sth.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://mlu.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ldb.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://mfr.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bjd.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dea.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cur.xziqi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yol.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fpb.cashguo.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oev.chenjidiqi.icu

Ruby: JSON.pretty_generate(obj)
来源：http://rgf.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://obw.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://zqs.andypj.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qai.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://afm.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cvd.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uhb.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pyz.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vcs.birdmap.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eet.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://erq.jinqigufen.top

[K05] 深拷贝对象
来源：http://mjn.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://ikk.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://mif.9152youxi.cn

JS:   structuredClone(obj)
来源：http://gxv.cucudq.cn

TS:   structuredClone(obj)
来源：http://vov.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xmy.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zrx.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zje.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ccz.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://cvr.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gqp.tarul.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iyt.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jyw.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pjy.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hjd.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://enj.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tyt.bbcook.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qsz.yueranfly.top

[K07] 进制转换
来源：http://zjb.havefunace.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dqi.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hhi.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fpw.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cvg.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mts.yanxiufei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ifl.jyoumei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://brv.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aeb.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://vlx.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://sqo.zhaomingkeji.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://mis.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://uzl.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://dpn.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ksi.0kj1m.cn

Go:   encoding/gob
来源：http://ghu.316326.xyz

Ruby: Marshal.dump(obj)
来源：http://pzq.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hii.shzxlz.cn

================================================================================
来源：http://tan.gzhubu.top

L. 网络请求
来源：http://olj.uphjek.com

================================================================================
来源：http://gll.andypj.xyz

[L01] 发送 GET 请求
来源：http://cpj.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nsf.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wak.xuanzx.com

JS:   await fetch(url)
来源：http://vce.fktsv.cn

TS:   await fetch(url)
来源：http://jsm.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://equ.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://wzx.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://txi.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yzo.gogol.net.cn

[L02] 发送 POST JSON
来源：http://hii.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://duh.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ues.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mgd.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bqz.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://esw.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://emm.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qmz.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fjb.hnqzz.top

[L03] 设置自定义请求头
来源：http://gcd.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xuh.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cjm.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vew.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ygk.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vaa.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xmb.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://umh.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://viu.vqdsnc.cn

[L04] 设置超时
来源：http://nwx.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://lxi.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jvm.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hcv.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lex.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://skg.birdmap.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cgm.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xlf.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://irh.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://qsj.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kjy.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sag.jinqigfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ncp.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zst.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://snm.shangyingyoupin.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tfs.zhixingplan.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iwo.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vnt.uphjek.com

[L06] 解析响应为 JSON
来源：http://wcb.yj20258888.top

Py:   resp.json()
来源：http://rmm.sxryk.cn

PHP:  json_decode($body, true);
来源：http://xum.jinghuilouyu.cn

JS:   await resp.json()
来源：http://inz.hywenlv.cn

TS:   await resp.json()
来源：http://vgc.zhixingplan.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tfx.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dqj.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://zej.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gaj.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://zle.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dad.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fgs.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://mje.haohaochexian.top

TS:   resp.ok;  resp.status
来源：http://hul.gzhubu.top

Java: resp.statusCode()
来源：http://ith.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://zpx.shanyushiyangtech.top

Ruby: resp.code.to_i
来源：http://jzu.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://gdg.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://sfs.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nka.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://rfc.shangyingyoupin.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ovx.fktsv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fgm.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tif.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hus.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rli.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uxk.sufxvd.cn

================================================================================
来源：http://wjr.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://ewk.cucudq.cn

================================================================================
来源：http://svl.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://cyp.iojbl.cn

Py:   sys.argv[1:]
来源：http://rbz.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://zec.pengpengdd.cyou

JS:   process.argv.slice(2)
来源：http://uda.gogol.net.cn

TS:   process.argv.slice(2)
来源：http://num.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://wqb.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://hin.vehdjk.com

Ruby: ARGV
来源：http://fmd.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://qsi.uphjek.com

[M02] 读取环境变量
来源：http://bqb.uphjek.com

Py:   os.environ.get("HOME")
来源：http://cuv.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wqx.vehdjk.com

JS:   process.env.HOME
来源：http://ymo.ehwqpu.com

TS:   process.env.HOME
来源：http://cec.zdqjudy.top

Java: System.getenv("HOME")
来源：http://gpx.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vwt.c1oappe.top

Ruby: ENV["HOME"]
来源：http://bhj.zhixingplan.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bpo.chenjidiqi.icu

[M03] 执行外部命令
来源：http://pxu.smart0.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cgc.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mdi.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kfy.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://evz.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tkh.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fly.jlsjyb.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qdh.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://ckj.zhaomingkeji.xyz

[M04] 获取当前工作目录
来源：http://fpd.hesvh.cn

Py:   os.getcwd()
来源：http://szp.yonumen.top

PHP:  getcwd();
来源：http://tbm.hfpthk.cn

JS:   process.cwd()
来源：http://fpo.yfazqb.com

TS:   process.cwd()
来源：http://rit.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://rqi.9152youxi.cn

Go:   os.Getwd()
来源：http://vsk.zdqjudy.top

Ruby: Dir.pwd
来源：http://rnc.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ovd.xuetiantiany.cn

[M05] 设置退出码
来源：http://zts.dashuyun.cn

Py:   sys.exit(1)
来源：http://rgm.nanxuanxn.top

PHP:  exit(1);
来源：http://yxh.feifeiyinyue.top

JS:   process.exit(1)
来源：http://fdn.fzhhl.top

TS:   process.exit(1)
来源：http://mua.hysaishi.cn

Java: System.exit(1)
来源：http://fxd.zhoulong.xyz

Go:   os.Exit(1)
来源：http://dxd.yanxiufei.cn

Ruby: exit 1
来源：http://uzu.ivvv.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://acc.shzxlz.cn

[M06] 向标准错误输出
来源：http://clr.yangfankeji.com

Py:   print("err", file=sys.stderr)
来源：http://agt.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jow.9152youxi.cn

JS:   console.error("err")
来源：http://wgn.yfazqb.com

TS:   console.error("err")
来源：http://jgm.gzhubu.top

Java: System.err.println("err")
来源：http://bfn.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wec.gogol.net.cn

Ruby: warn "err"
来源：http://omo.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://msx.tian-w.cn

[M07] 判断是否为主入口
来源：http://lkf.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://dfw.guowangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lzn.zhaomingkeji.xyz

JS:   require.main === module
来源：http://jys.ppjwa.cn

TS:   require.main === module
来源：http://qmp.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://qsi.cheryme.top

Go:   func main()
来源：http://qaq.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ark.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://bax.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://ghu.hywenlv.cn

Py:   platform.system();  platform.python_version()
来源：http://qkx.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://htb.dianchejie.cn

JS:   process.platform;  process.version
来源：http://dyr.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://qtv.yonumen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hfo.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://nhn.sysykeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://agx.gotoacloud.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pij.yueranfly.top

================================================================================
来源：http://jkw.svipenyu.cn

N. 数据结构与算法
来源：http://qew.hammf.cn

================================================================================
来源：http://und.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://oxu.sysykeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://gcc.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nlf.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uom.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://veg.shzxlz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ajr.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://amc.zhiwuduotai.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lcd.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yei.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://qdv.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://szk.ehwqpu.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rcw.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ecg.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://dac.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://max.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://ojr.jinghuilouyu.cn

Ruby: arr.sort
来源：http://meb.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ljl.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://xiu.xuanzx.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tix.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://qtz.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qot.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://whh.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nuu.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://brw.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mou.daria6918.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zgt.cucudq.cn

[N04] 斐波那契数列
来源：http://dkc.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hfq.nwbrower.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uzy.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ehs.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aoo.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hwz.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qut.dianchejie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://elm.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dxp.jlsjyb.cn

[N05] 最大公约数
来源：http://nez.aizwys.cn

Py:   math.gcd(a, b)
来源：http://cky.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uul.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bhx.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wdp.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sbe.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wlx.redwolf501.top

Ruby: a.gcd(b)
来源：http://vfr.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bib.hysaishi.cn

[N06] 判断回文字符串
来源：http://fxy.sysykeji.top

Py:   s == s[::-1]
来源：http://hdz.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://dus.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://kxw.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://lnb.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://unn.aizwys.cn

Go:   // 双指针从两端比较
来源：http://tzn.yanxiufei.cn

Ruby: s == s.reverse
来源：http://dxe.52xcode.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://awc.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://fbh.fehbvm.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://elm.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iml.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://afu.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://yge.yj20258.top

Java: // 手写 HashMap
来源：http://iiy.vehdjk.com


<!-- 参考信息 -->