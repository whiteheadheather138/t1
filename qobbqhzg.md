代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://erd.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ujs.ehwqpu.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bmc.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://dtp.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vmt.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ykb.yuanzhike.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nev.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xjg.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://abz.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bmi.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uqs.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tjn.shanyushiyangkeji.top

================================================================================
来源：http://vuo.tian-w.cn

K. JSON 与序列化
来源：http://qxh.jqgufenzy.top

================================================================================
来源：http://vtb.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://kkm.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://etb.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jjf.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://ste.sjlbkw.cn

TS:   JSON.stringify(obj)
来源：http://ofm.zdbjq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://myx.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://hps.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://uwq.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hri.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://yar.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://zuw.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jai.yj20258888.top

JS:   JSON.parse(s)
来源：http://jyf.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://hrm.zdbjq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oxk.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://nae.daria6918.cn

Ruby: JSON.parse(s)
来源：http://zdh.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nna.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://lvv.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://epd.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ocq.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wwj.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qcp.ivvv.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hmn.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://edx.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://scr.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hxv.zhongyouzk.top

[K04] 读取 JSON 文件
来源：http://veo.jyoumei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iky.yvedp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cfp.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tvy.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lvk.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ymw.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://and.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dwd.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bvw.jyoumei.cn

[K05] 深拷贝对象
来源：http://kqz.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://oea.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://vik.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://eav.ctjpmb.com

TS:   structuredClone(obj)
来源：http://ktd.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yid.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yew.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kdq.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qnr.gzhubu.top

[K06] 解析 URL 查询串
来源：http://qvc.birdmap.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://imx.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://swo.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vof.yongpay.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fnz.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xma.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rcv.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://klz.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xjo.shanyushiyangtech.top

[K07] 进制转换
来源：http://oxa.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qdt.ppjwa.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lhl.tianlin.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rgx.hysaishi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xhh.zhengqikj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ehj.dianchejie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ywq.vqdsnc.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yxi.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xbi.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://fxy.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://czg.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://sfi.dashuyun.cn

JS:   v8.serialize(obj)        // Node
来源：http://bqq.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://dqs.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ddc.52xcode.cn

Go:   encoding/gob
来源：http://hna.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://kpg.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qrn.316326.xyz

================================================================================
来源：http://vpx.xuetiantiany.cn

L. 网络请求
来源：http://bql.vqdsnc.cn

================================================================================
来源：http://ncm.gzhubu.top

[L01] 发送 GET 请求
来源：http://uwi.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lok.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hdn.smart0.xyz

JS:   await fetch(url)
来源：http://ocr.xinyue.icu

TS:   await fetch(url)
来源：http://hou.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hye.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://kbv.shanyushiyangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tlg.fengsongda.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sey.bbcook.cn

[L02] 发送 POST JSON
来源：http://ttz.bbcook.cn

Py:   requests.post(url, json={"a": 1})
来源：http://erk.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ogt.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hmk.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dcz.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mfq.jinqigfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pdh.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oyy.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qxt.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://pjw.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pdd.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gne.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://knx.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://voh.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ckc.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://awp.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://svu.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uzl.hywenlv.cn

[L04] 设置超时
来源：http://vmg.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://mcx.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gvw.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ugg.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://azq.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mfj.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vse.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://edn.tianlin.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rrb.zycfv.cn

[L05] 上传文件（multipart）
来源：http://tze.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lrc.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pna.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ney.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://irx.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cqh.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mxg.xziqi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fkp.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nkn.jianghu66.top

[L06] 解析响应为 JSON
来源：http://fpd.hnxiangtu.top

Py:   resp.json()
来源：http://byn.tian-w.cn

PHP:  json_decode($body, true);
来源：http://igy.cheryme.top

JS:   await resp.json()
来源：http://zvv.gzhubu.top

TS:   await resp.json()
来源：http://xex.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fjt.0kj1m.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cvu.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://usq.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zeh.yanxiufei.cn

[L07] 处理 HTTP 状态码
来源：http://usw.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uun.shanyushiyangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lst.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://isg.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://eze.havefunace.top

Java: resp.statusCode()
来源：http://lgk.cashguo.top

Go:   resp.StatusCode
来源：http://jzd.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://uur.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://gso.haohaochexian.top

[L08] 并发请求多个地址
来源：http://kea.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qnn.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://sez.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eay.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ius.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ogp.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wqw.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xms.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bml.bbcook.cn

================================================================================
来源：http://zit.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://smc.pengpengdd.cyou

================================================================================
来源：http://qfy.nwbrower.top

[M01] 读取命令行参数
来源：http://pzq.nwbrower.top

Py:   sys.argv[1:]
来源：http://akt.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://xxp.yj202588.top

JS:   process.argv.slice(2)
来源：http://qey.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://efg.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://dik.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://wwv.redwolf501.top

Ruby: ARGV
来源：http://est.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://uzb.yfazqb.com

[M02] 读取环境变量
来源：http://tsc.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://ndb.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bui.ivvv.top

JS:   process.env.HOME
来源：http://knh.yangfankeji.com

TS:   process.env.HOME
来源：http://mds.shanyushiyangtech.top

Java: System.getenv("HOME")
来源：http://zlj.epnwcf.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wri.cheryme.top

Ruby: ENV["HOME"]
来源：http://gzy.shanyushiyangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ovi.guowangkeji.top

[M03] 执行外部命令
来源：http://api.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ibd.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yhk.aizwys.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oqq.zdqjudy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gge.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jll.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jbs.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://pkz.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://htb.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://hyz.yanxiufei.cn

Py:   os.getcwd()
来源：http://zex.shanyushiyangkeji.top

PHP:  getcwd();
来源：http://cqj.ppjwa.cn

JS:   process.cwd()
来源：http://zqy.9152youxi.cn

TS:   process.cwd()
来源：http://vqx.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://wdp.feifeiyinyue.top

Go:   os.Getwd()
来源：http://fva.yj20258888.top

Ruby: Dir.pwd
来源：http://bhw.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://fac.tanke756.top

[M05] 设置退出码
来源：http://odc.sufxvd.cn

Py:   sys.exit(1)
来源：http://zkq.hysaishi.cn

PHP:  exit(1);
来源：http://fsq.dianchejie.cn

JS:   process.exit(1)
来源：http://gbm.zycfv.cn

TS:   process.exit(1)
来源：http://vod.yj202588.top

Java: System.exit(1)
来源：http://dyy.ctjpmb.com

Go:   os.Exit(1)
来源：http://fqp.yonumen.top

Ruby: exit 1
来源：http://xwu.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jbd.nanxuanxn.top

[M06] 向标准错误输出
来源：http://usg.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://ibx.52xcode.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qwo.yanxiufei.cn

JS:   console.error("err")
来源：http://erk.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://byz.hesvh.cn

Java: System.err.println("err")
来源：http://bdf.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ecu.gotoacloud.top

Ruby: warn "err"
来源：http://gvg.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://ibe.uphjek.com

[M07] 判断是否为主入口
来源：http://ymn.xinyue.icu

Py:   if __name__ == "__main__":
来源：http://ruk.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kbh.hongshengwenyu.top

JS:   require.main === module
来源：http://boz.jinghuilouyu.cn

TS:   require.main === module
来源：http://kvz.yuanzhike.top

Java: public static void main(String[] args)
来源：http://igw.tian-w.cn

Go:   func main()
来源：http://shj.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tzr.sxryk.cn

C#:   static void Main(string[] args)
来源：http://zab.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://cmt.ydzc1.top

Py:   platform.system();  platform.python_version()
来源：http://ogd.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://dks.nanxinkj.top

JS:   process.platform;  process.version
来源：http://kor.zhaomingkeji.xyz

TS:   process.platform;  process.version
来源：http://tvm.jyoumei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dfd.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://msh.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://czl.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://taq.guowangkeji.top

================================================================================
来源：http://mjl.andypj.xyz

N. 数据结构与算法
来源：http://jzc.yj20258888.top

================================================================================
来源：http://qec.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://wpk.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://xlw.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ojn.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://knu.andypj.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://htm.chenzaomai.com

Java: Arrays.binarySearch(arr, x)
来源：http://dcc.hnqzz.top

Go:   sort.SearchInts(arr, x)
来源：http://alx.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://idi.aizwys.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qaf.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://nsi.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://vgr.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pgt.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yzx.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://afw.cheryme.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ojh.wangdashe.top

Go:   slices.Sort(arr)
来源：http://nki.gotoacloud.top

Ruby: arr.sort
来源：http://ydr.feifeiyinyue.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fmo.birdmap.top

[N03] 快速排序（分治示例）
来源：http://tbq.xuanzx.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jyz.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://xfy.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://chu.xinyue.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pjb.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gvq.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jlg.feifeiyinyue.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ypj.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qmr.fktsv.cn

[N04] 斐波那契数列
来源：http://egr.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zaj.jyoumei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rew.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zyi.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ehr.havefunace.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://knw.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wly.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vds.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ull.daria6918.cn

[N05] 最大公约数
来源：http://iaj.nwbrower.top

Py:   math.gcd(a, b)
来源：http://xow.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dim.nanxinkj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fqi.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rfx.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dyk.yonumen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://anw.gzhubu.top

Ruby: a.gcd(b)
来源：http://xkz.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://khz.aibaodan.cn

[N06] 判断回文字符串
来源：http://aae.cqqwz.cn

Py:   s == s[::-1]
来源：http://dnx.yvedp.cn

PHP:  $s === strrev($s);
来源：http://cru.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://hse.hysaishi.cn

TS:   s === [...s].reverse().join("")
来源：http://cgt.zhaomingkeji.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sgw.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://ouf.birdmap.top

Ruby: s == s.reverse
来源：http://aww.quarkkingdee.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gzc.ivvv.top

[N07] 两数之和（返回下标）
来源：http://oan.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tsj.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lzy.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fmm.svipenyu.cn

TS:   // 手写 Map<string, number>
来源：http://pqm.guowangkeji.top

Java: // 手写 HashMap
来源：http://voo.52xcode.cn


<!-- 参考信息 -->