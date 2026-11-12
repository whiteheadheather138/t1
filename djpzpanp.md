代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://dyr.shuidangran.top

[J08] 提取年月日与星期
来源：http://htq.daria6918.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kxa.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ffq.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aht.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bvg.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jcz.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tkf.hammf.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wdo.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://obp.havefunace.top

[J09] 时区处理
来源：http://fac.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aue.ivvv.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bzj.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://irm.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gyl.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mld.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yum.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://svf.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pij.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://pui.pengpengdd.cyou

Py:   date.today();  date.today().replace(day=1)
来源：http://vzh.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mts.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mnu.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tte.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xpo.pengpengdd.cyou

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ayu.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gbs.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lol.jinqigfzy.top

================================================================================
来源：http://ujh.vqdsnc.cn

K. JSON 与序列化
来源：http://vou.xylfe.cn

================================================================================
来源：http://qer.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://oth.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://scb.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cjm.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://vhv.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://bwy.jlsjyb.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yje.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://rkr.guowangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://vym.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vab.havefunace.top

[K02] JSON 字符串转对象
来源：http://jgd.yuxming.cn

Py:   json.loads(s)
来源：http://aww.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xsh.fktsv.cn

JS:   JSON.parse(s)
来源：http://feh.shuidangran.top

TS:   JSON.parse(s)
来源：http://ift.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ite.quarkkingdee.top

Go:   json.Unmarshal(data, &v)
来源：http://whb.gogol.net.cn

Ruby: JSON.parse(s)
来源：http://rlq.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ncz.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://cwo.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mmk.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fml.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gqf.hfpthk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qow.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tao.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gij.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://oxk.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bks.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://hky.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ifh.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mns.redwolf501.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hsq.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ywf.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dru.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://phq.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://iiy.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zwk.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://iid.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://fsi.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://wyo.gaohongyu789.top

JS:   structuredClone(obj)
来源：http://mpf.tian-w.cn

TS:   structuredClone(obj)
来源：http://suj.cashguo.top

Java: // 手写拷贝构造，或序列化往返
来源：http://owq.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bop.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dnm.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://wen.svipenyu.cn

[K06] 解析 URL 查询串
来源：http://asv.sxryk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fgv.kuanghao11.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ioe.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nnc.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kde.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ybm.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://pbt.ybcxt.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aqk.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xsv.0kj1m.cn

[K07] 进制转换
来源：http://jek.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zcj.smart0.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gei.hesvh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://utk.shangyingyoupin.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ijo.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fpc.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gum.haohaochexian.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kuc.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bdx.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://uck.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://jex.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lyz.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://bpv.guowangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://rcy.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nrh.wangshuangyany.cn

Go:   encoding/gob
来源：http://fpr.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://dpz.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kuu.gzhubu.top

================================================================================
来源：http://abv.chenzaomai.com

L. 网络请求
来源：http://bvs.c1oappe.top

================================================================================
来源：http://wnx.jqgfzy.top

[L01] 发送 GET 请求
来源：http://rdm.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dvn.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://skf.zhoulong.xyz

JS:   await fetch(url)
来源：http://rpg.zdqjudy.top

TS:   await fetch(url)
来源：http://cyk.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ypa.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://yxv.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://noy.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nfu.yonumen.top

[L02] 发送 POST JSON
来源：http://vpe.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://kog.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://clw.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://edz.andypj.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tjz.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gme.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zle.jianghu66.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uqx.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wag.haohaochexian.top

[L03] 设置自定义请求头
来源：http://hhz.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cdo.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ysb.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hxt.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jcz.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wxj.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dry.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nwj.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://buz.sufxvd.cn

[L04] 设置超时
来源：http://jxz.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://zhc.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iuq.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hqo.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gjb.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wcl.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ppw.ydjk.org.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://csu.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pqr.yongpay.top

[L05] 上传文件（multipart）
来源：http://ndf.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://juv.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fhj.smart0.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ufo.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://paw.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tdm.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jpo.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://onn.iojbl.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eej.sysykeji.top

[L06] 解析响应为 JSON
来源：http://ztc.fanxiaobao.xyz

Py:   resp.json()
来源：http://mgv.tianlin.xyz

PHP:  json_decode($body, true);
来源：http://auv.yueranfly.top

JS:   await resp.json()
来源：http://tjc.hcnkem.com

TS:   await resp.json()
来源：http://syu.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nxd.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ebw.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://wbx.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ejv.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://ywk.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oeu.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hst.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://rdk.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://pgm.chenzaomai.com

Java: resp.statusCode()
来源：http://bqt.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://mpi.yonumen.top

Ruby: resp.code.to_i
来源：http://uyi.ppjwa.cn

C#:   (int)resp.StatusCode
来源：http://ged.jqgufenzy.top

[L08] 并发请求多个地址
来源：http://vne.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vnb.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://usl.ydzc1.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://woo.hywenlv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qby.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eut.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hnv.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sjq.birdmap.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gqr.shanyushiyangtech.top

================================================================================
来源：http://mik.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://yam.aizwys.cn

================================================================================
来源：http://ezy.cashguo.top

[M01] 读取命令行参数
来源：http://djv.zhixingplan.top

Py:   sys.argv[1:]
来源：http://yfp.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://zyo.sweek.top

JS:   process.argv.slice(2)
来源：http://kqg.ivvv.top

TS:   process.argv.slice(2)
来源：http://agh.gzhubu.top

Java: args 数组（main 方法参数）
来源：http://gsi.jinghuilouyu.cn

Go:   os.Args[1:]
来源：http://egf.cucudq.cn

Ruby: ARGV
来源：http://nri.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://dkm.ydzc1.top

[M02] 读取环境变量
来源：http://eia.hnxiangtu.top

Py:   os.environ.get("HOME")
来源：http://gjn.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lca.guannengcc.top

JS:   process.env.HOME
来源：http://fcd.sufxvd.cn

TS:   process.env.HOME
来源：http://lmf.jiagoushi.top

Java: System.getenv("HOME")
来源：http://fjn.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ade.uphjek.com

Ruby: ENV["HOME"]
来源：http://lcc.cqqwz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dkb.yanxiufei.cn

[M03] 执行外部命令
来源：http://kqv.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xzu.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fcv.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wjd.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dug.tian-w.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ufc.hnqzz.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jxf.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dtj.fanxiaobao.xyz

C#:   Process.Start("ls", "-l");
来源：http://ixb.zdbjq.cn

[M04] 获取当前工作目录
来源：http://fuk.daria6918.cn

Py:   os.getcwd()
来源：http://cux.sysykeji.top

PHP:  getcwd();
来源：http://nzh.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://jta.zhengqikj.top

TS:   process.cwd()
来源：http://vfq.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://ywr.redwolf501.top

Go:   os.Getwd()
来源：http://nfk.daria6918.cn

Ruby: Dir.pwd
来源：http://wbc.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://get.birdmap.top

[M05] 设置退出码
来源：http://ulo.chenjidiqi.icu

Py:   sys.exit(1)
来源：http://fou.xuetiantiany.cn

PHP:  exit(1);
来源：http://gqy.iojbl.cn

JS:   process.exit(1)
来源：http://ben.iojbl.cn

TS:   process.exit(1)
来源：http://ixf.uphjek.com

Java: System.exit(1)
来源：http://djk.sxryk.cn

Go:   os.Exit(1)
来源：http://ovr.hywenlv.cn

Ruby: exit 1
来源：http://fai.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xdb.snrcjt.cn

[M06] 向标准错误输出
来源：http://jca.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://bvu.cashguo.top

PHP:  fwrite(STDERR, "err\n");
来源：http://udt.jinghuilouyu.cn

JS:   console.error("err")
来源：http://ewf.316326.xyz

TS:   console.error("err")
来源：http://mky.fktsv.cn

Java: System.err.println("err")
来源：http://hgi.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oqt.jyoumei.cn

Ruby: warn "err"
来源：http://twx.ppjwa.cn

C#:   Console.Error.WriteLine("err")
来源：http://yml.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://hoi.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://gbi.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cuc.shuidangran.top

JS:   require.main === module
来源：http://vvf.jianghu66.top

TS:   require.main === module
来源：http://sdl.jianghu66.top

Java: public static void main(String[] args)
来源：http://gap.hesvh.cn

Go:   func main()
来源：http://gyo.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wlu.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://uci.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://mjg.zhijiandao.cn

Py:   platform.system();  platform.python_version()
来源：http://xfy.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://vdf.fanxiaobao.xyz

JS:   process.platform;  process.version
来源：http://pjp.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://tcg.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vbo.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://yde.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://upd.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nmr.shzxlz.cn

================================================================================
来源：http://tuf.hongshengwenyu.top

N. 数据结构与算法
来源：http://wih.jinyuanbaomall.cn

================================================================================
来源：http://fne.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://kkh.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://reh.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dtj.shanyushiyangtech.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fza.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ogt.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ktm.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://krq.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zfd.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pfp.yueranfly.top

[N02] 排序（工程实践用内置实现）
来源：http://uzs.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://unw.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ull.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nve.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mlo.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sak.zycfv.cn

Go:   slices.Sort(arr)
来源：http://jkt.vqdsnc.cn

Ruby: arr.sort
来源：http://qoa.gaohongyu789.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gdy.hammf.cn

[N03] 快速排序（分治示例）
来源：http://qcn.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jli.hammf.cn

PHP:  // 递归实现，或用 usort
来源：http://ugi.sweek.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oeh.meibo888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ols.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://amf.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://btm.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uiy.shanyushiyangtech.top

C#:   // 手写递归，或 Array.Sort
来源：http://ser.jyoumei.cn

[N04] 斐波那契数列
来源：http://qbf.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://scc.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mgu.yueranfly.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mae.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tcj.ydjk.org.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rfb.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ecz.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ewq.hnqzz.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jus.nwbrower.top

[N05] 最大公约数
来源：http://ujg.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://jcd.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jwe.shangyingyoupin.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tww.kuanghao11.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xow.guannengcc.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rql.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bxc.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://isv.fanxiaobao.xyz


<!-- 参考信息 -->