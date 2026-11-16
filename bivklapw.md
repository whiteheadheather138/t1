代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://nen.aibaodan.cn

[J08] 提取年月日与星期
来源：http://igg.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://obj.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fyp.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xml.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://col.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tux.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sfk.yueranfly.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tsj.jianghu66.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pvf.uphjek.com

[J09] 时区处理
来源：http://ubh.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dnq.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oil.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bhj.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gcc.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vxu.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ove.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://aap.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fmh.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://wpx.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cec.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lqj.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yla.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sqw.fzhhl.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://krd.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kiv.tanke756.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bqu.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mug.yvedp.cn

================================================================================
来源：http://zzo.epnwcf.com

K. JSON 与序列化
来源：http://yof.jlsjyb.cn

================================================================================
来源：http://jja.xuetiantiany.cn

[K01] 对象转 JSON 字符串
来源：http://tvk.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pqa.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gkh.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://msx.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://zql.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bdy.fzhhl.top

Go:   json.Marshal(obj)
来源：http://tyy.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gnw.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pal.shuidangran.top

[K02] JSON 字符串转对象
来源：http://yxc.fzhhl.top

Py:   json.loads(s)
来源：http://jfr.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://smb.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://heo.sweek.top

TS:   JSON.parse(s)
来源：http://xay.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://byb.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://sdt.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://yqy.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hev.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://lri.feifeiyinyue.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kxa.hfpthk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ynw.ybcxt.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oob.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://hip.redwolf501.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fyo.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wyl.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://uld.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tri.havefunace.top

[K04] 读取 JSON 文件
来源：http://ayv.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://koj.sweek.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fbx.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xtl.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lhd.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fic.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ktu.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gdb.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wbu.guannengcc.top

[K05] 深拷贝对象
来源：http://yai.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://eib.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://smo.fzhhl.top

JS:   structuredClone(obj)
来源：http://pqd.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://doe.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qma.daxiang520.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iak.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://izx.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ssw.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://uvb.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wiv.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://now.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sfn.epnwcf.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://osx.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://asf.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://dov.quarkkingdee.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sbj.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kjb.aibaodan.cn

[K07] 进制转换
来源：http://ayg.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fnd.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ozk.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zvk.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kls.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vmz.mhx1999.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ovp.mhx1999.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bqq.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vns.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://mkt.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://ypa.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ahl.c1oappe.top

JS:   v8.serialize(obj)        // Node
来源：http://oab.hnxiangtu.top

TS:   v8.serialize(obj)        // Node
来源：http://jba.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bap.jqgufenzy.top

Go:   encoding/gob
来源：http://kgr.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://sgc.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://usx.tarul.cn

================================================================================
来源：http://ybm.shanyushiyangtech.top

L. 网络请求
来源：http://fws.nwbrower.top

================================================================================
来源：http://vvn.shuidangran.top

[L01] 发送 GET 请求
来源：http://dhm.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://esy.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rak.zdbjq.cn

JS:   await fetch(url)
来源：http://lev.aibaodan.cn

TS:   await fetch(url)
来源：http://dxo.vehdjk.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nsl.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://owo.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://kzn.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://myh.shuidangran.top

[L02] 发送 POST JSON
来源：http://tuu.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hng.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gzn.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://khh.jianghu66.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fzu.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nif.andypj.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pwq.fehbvm.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hbi.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://shx.cdnleiting.top

[L03] 设置自定义请求头
来源：http://wag.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kgl.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tlf.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jad.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eun.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tvk.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fry.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eul.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ibj.hysaishi.cn

[L04] 设置超时
来源：http://rba.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://fuh.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://prt.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bib.sufxvd.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ztq.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rxz.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hul.tanke756.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bgc.yuanzhike.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cmw.ivvv.top

[L05] 上传文件（multipart）
来源：http://gux.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://udy.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mjt.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ljf.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yzj.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eim.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iok.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://moj.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tij.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://ucy.shuidangran.top

Py:   resp.json()
来源：http://tqo.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://etk.jinqigfzy.top

JS:   await resp.json()
来源：http://kmm.xuanzx.com

TS:   await resp.json()
来源：http://vra.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://arx.daria6918.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jzo.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://fkp.sufxvd.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rlu.yj20258888.top

[L07] 处理 HTTP 状态码
来源：http://gug.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vzx.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bzz.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://mcn.yuxming.cn

TS:   resp.ok;  resp.status
来源：http://pyz.jinqigfzy.top

Java: resp.statusCode()
来源：http://otn.xingfuxueyuan.xyz

Go:   resp.StatusCode
来源：http://zgv.sjlbkw.cn

Ruby: resp.code.to_i
来源：http://kyz.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://nve.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://ubr.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wpa.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://ofr.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pcl.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ooy.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://frk.hesvh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lfy.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jbz.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ckt.ivvv.top

================================================================================
来源：http://kfs.cucudq.cn

M. 命令行 / 进程 / 环境
来源：http://pbp.yonumen.top

================================================================================
来源：http://qmj.ivvv.top

[M01] 读取命令行参数
来源：http://vsn.jiagoushi.top

Py:   sys.argv[1:]
来源：http://ffn.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://uhk.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://yxy.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://cfd.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://yut.hnxiangtu.top

Go:   os.Args[1:]
来源：http://kte.dashuyun.cn

Ruby: ARGV
来源：http://uul.nwbrower.top

C#:   args 数组（Main 方法参数）
来源：http://zki.zhongyouzk.top

[M02] 读取环境变量
来源：http://jda.yonumen.top

Py:   os.environ.get("HOME")
来源：http://yxu.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yzd.svipenyu.cn

JS:   process.env.HOME
来源：http://nui.snrcjt.cn

TS:   process.env.HOME
来源：http://zzj.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://xhd.hywenlv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gyj.bjfxy.top

Ruby: ENV["HOME"]
来源：http://man.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zpk.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://yau.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tai.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://umm.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://obe.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://qyy.ppjwa.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vnn.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nvr.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://bva.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://pli.yueranfly.top

[M04] 获取当前工作目录
来源：http://xvc.xuetiantiany.cn

Py:   os.getcwd()
来源：http://ksr.nanxuanxn.top

PHP:  getcwd();
来源：http://xii.vqdsnc.cn

JS:   process.cwd()
来源：http://trq.zhijiandao.cn

TS:   process.cwd()
来源：http://zui.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://npz.cashguo.top

Go:   os.Getwd()
来源：http://clj.vehdjk.com

Ruby: Dir.pwd
来源：http://umg.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://uki.epnwcf.com

[M05] 设置退出码
来源：http://ebb.cashguo.top

Py:   sys.exit(1)
来源：http://xvi.cashguo.top

PHP:  exit(1);
来源：http://ddy.ivvv.top

JS:   process.exit(1)
来源：http://vlw.9152youxi.cn

TS:   process.exit(1)
来源：http://xle.yfazqb.com

Java: System.exit(1)
来源：http://riy.gaohongyu789.top

Go:   os.Exit(1)
来源：http://xki.gaohongyu789.top

Ruby: exit 1
来源：http://xrv.ivvv.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pae.kuanghao11.cn

[M06] 向标准错误输出
来源：http://pqz.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://fzc.hfpthk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rjl.wangdashe.top

JS:   console.error("err")
来源：http://tci.chenzaomai.com

TS:   console.error("err")
来源：http://ehc.xylfe.cn

Java: System.err.println("err")
来源：http://jst.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lpb.yangfankeji.com

Ruby: warn "err"
来源：http://omx.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://gun.tarul.cn

[M07] 判断是否为主入口
来源：http://hxg.birdmap.top

Py:   if __name__ == "__main__":
来源：http://grs.sxryk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://weq.snrcjt.cn

JS:   require.main === module
来源：http://dqw.aibaodan.cn

TS:   require.main === module
来源：http://tjb.fengsongda.top

Java: public static void main(String[] args)
来源：http://lmn.0kj1m.cn

Go:   func main()
来源：http://uyk.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qtr.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://tcb.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://wmi.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://hjc.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://jgm.xuanzx.com

JS:   process.platform;  process.version
来源：http://ttd.gaohongyu789.top

TS:   process.platform;  process.version
来源：http://ysr.dashuyun.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oqn.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dns.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mdb.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wis.zhixingplan.top

================================================================================
来源：http://jky.dianchejie.cn

N. 数据结构与算法
来源：http://cjo.shzxlz.cn

================================================================================
来源：http://ter.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://wjv.vqdsnc.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yoi.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ukn.fktsv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wkw.sufxvd.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://deb.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://hot.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://xug.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uxc.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://vbd.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://eve.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://nzr.aibaodan.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rqd.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://oyv.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tff.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bay.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://bep.fktsv.cn

Ruby: arr.sort
来源：http://xtp.tanke756.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zkc.yfazqb.com

[N03] 快速排序（分治示例）
来源：http://shb.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ggc.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://xii.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qya.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eyc.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nuu.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rdi.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wfy.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pba.shzxlz.cn

[N04] 斐波那契数列
来源：http://rmm.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://icd.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vzs.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ynq.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xtw.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xqo.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tuv.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cgr.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lbx.zhoulong.xyz

[N05] 最大公约数
来源：http://zxz.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://yyt.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hfs.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rjt.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pij.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vmz.ydjk.org.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rtd.yuanzhike.top

Ruby: a.gcd(b)
来源：http://inf.fengsongda.top


<!-- 参考信息 -->