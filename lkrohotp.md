代发 wailian999

Py:   (end - start).total_seconds()
来源：http://uxh.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://xbx.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ton.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ide.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://iqo.fehbvm.com

Go:   end.Sub(start).Hours()
来源：http://lmz.sweek.top

Ruby: end - start                 # 返回秒数
来源：http://fbh.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://zcy.feifeiyinyue.top

[J07] 比较两个日期
来源：http://noa.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://wzv.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qxj.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mhw.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uer.yj202588.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://exl.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jab.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://evn.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://obq.daxiang520.top

[J08] 提取年月日与星期
来源：http://lrp.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://azw.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://asy.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zct.gaohongyu789.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://civ.zhijiandao.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aws.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xri.sjlbkw.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dje.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jye.yangfankeji.com

[J09] 时区处理
来源：http://pnd.pycfn.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iov.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cuf.gotoacloud.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ozm.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ysl.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://guo.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tml.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zuc.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hdy.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://mso.smart0.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://xao.fanxiaobao.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://flm.kuanghao11.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xcy.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qdv.zhixingplan.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bgw.52xcode.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nom.andypj.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vum.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tgg.ydjk.org.cn

================================================================================
来源：http://vih.zhijiandao.cn

K. JSON 与序列化
来源：http://btg.cashguo.top

================================================================================
来源：http://ulx.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://kqz.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ure.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pos.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://rzj.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://abe.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://upv.52xcode.cn

Go:   json.Marshal(obj)
来源：http://nmy.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oig.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zwl.jyoumei.cn

[K02] JSON 字符串转对象
来源：http://wxk.yueranfly.top

Py:   json.loads(s)
来源：http://zrw.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://duy.zhijiandao.cn

JS:   JSON.parse(s)
来源：http://yiz.yueranfly.top

TS:   JSON.parse(s)
来源：http://zex.jqgfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ivg.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://csm.ywan-chungtsiang.top

Ruby: JSON.parse(s)
来源：http://qdc.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wrp.ydjk.org.cn

[K03] JSON 美化输出（带缩进）
来源：http://ocq.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dut.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ucq.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gmj.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gvd.ywan-chungtsiang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rtn.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qap.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ueq.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jqy.epnwcf.com

[K04] 读取 JSON 文件
来源：http://hlq.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dhk.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bkv.yuxming.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://occ.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://arc.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zhf.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gov.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://wvu.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qft.zdqjudy.top

[K05] 深拷贝对象
来源：http://hlw.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://mca.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://awh.xziqi.cn

JS:   structuredClone(obj)
来源：http://hsk.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://cwl.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bpf.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://saq.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xqw.vqdsnc.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tfd.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://dro.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eow.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nlz.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ryr.sweek.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tyo.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mmn.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hte.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zfp.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mcf.nanxinkj.top

[K07] 进制转换
来源：http://czg.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oko.daria6918.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vyv.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dzq.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ekj.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cch.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://trn.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xbt.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zlv.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://zkb.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://yrm.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://unv.meibo888.top

JS:   v8.serialize(obj)        // Node
来源：http://igg.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://zah.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pnj.redwolf501.top

Go:   encoding/gob
来源：http://ssy.uphjek.com

Ruby: Marshal.dump(obj)
来源：http://eoj.xuanzx.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qrc.fanxiaobao.xyz

================================================================================
来源：http://fks.nanxinkj.top

L. 网络请求
来源：http://amh.zdqjudy.top

================================================================================
来源：http://kql.yj20258.top

[L01] 发送 GET 请求
来源：http://uru.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lhb.quarkkingdee.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://umb.ivvv.top

JS:   await fetch(url)
来源：http://zrj.guannengcc.top

TS:   await fetch(url)
来源：http://qwj.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uyr.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://izj.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ics.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://chu.ctjpmb.com

[L02] 发送 POST JSON
来源：http://abs.dashuyun.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kal.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wgv.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lfg.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gui.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xgb.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lqb.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tas.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rdf.birdmap.top

[L03] 设置自定义请求头
来源：http://xia.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tdx.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kvl.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sju.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://amt.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sar.zdbjq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uze.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vlm.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kwr.zhaomingkeji.xyz

[L04] 设置超时
来源：http://ehr.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://pzx.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pyw.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vae.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ckg.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zvg.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tkb.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://seh.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://noa.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://ebv.jinqigfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rdm.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wgk.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kgy.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zuc.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xvz.tian-w.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://brx.jinghuilouyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://swo.hongshengwenyu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://icj.cashguo.top

[L06] 解析响应为 JSON
来源：http://nnk.zdbjq.cn

Py:   resp.json()
来源：http://dvt.316326.xyz

PHP:  json_decode($body, true);
来源：http://rni.316326.xyz

JS:   await resp.json()
来源：http://scz.316326.xyz

TS:   await resp.json()
来源：http://qob.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xoo.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dyw.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://dhf.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hcb.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://eqt.daxiang520.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tad.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://upz.hnxiangtu.top

JS:   resp.ok;  resp.status
来源：http://fnc.daria6918.cn

TS:   resp.ok;  resp.status
来源：http://aep.tianlin.xyz

Java: resp.statusCode()
来源：http://umq.cqqwz.cn

Go:   resp.StatusCode
来源：http://vvr.52xcode.cn

Ruby: resp.code.to_i
来源：http://xkd.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://gle.nwbrower.top

[L08] 并发请求多个地址
来源：http://izl.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://feu.redwolf501.top

PHP:  curl_multi_init() 系列
来源：http://fpb.andypj.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rjy.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qdr.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fru.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tcz.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://puy.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tmt.dianchejie.cn

================================================================================
来源：http://mvd.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://wqu.xingfuxueyuan.xyz

================================================================================
来源：http://ima.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://fas.daxiang520.top

Py:   sys.argv[1:]
来源：http://ood.meibo888.top

PHP:  $argv;  $argc;
来源：http://cyd.epnwcf.com

JS:   process.argv.slice(2)
来源：http://iqv.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://tli.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://wsd.yongpay.top

Go:   os.Args[1:]
来源：http://gnz.havefunace.top

Ruby: ARGV
来源：http://mxb.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://avs.zhoulong.xyz

[M02] 读取环境变量
来源：http://wnn.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://chj.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dmm.zhengqikj.top

JS:   process.env.HOME
来源：http://xzk.svipenyu.cn

TS:   process.env.HOME
来源：http://dlu.ivvv.top

Java: System.getenv("HOME")
来源：http://yta.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fpb.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://xic.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lel.shzxlz.cn

[M03] 执行外部命令
来源：http://edp.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hyw.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pix.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://qql.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://pff.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rbh.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cys.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://gqu.zhaomingkeji.xyz

C#:   Process.Start("ls", "-l");
来源：http://xzo.uphjek.com

[M04] 获取当前工作目录
来源：http://iqw.316326.xyz

Py:   os.getcwd()
来源：http://diy.c1oappe.top

PHP:  getcwd();
来源：http://zzu.chenlongwang.top

JS:   process.cwd()
来源：http://dij.guowangkeji.top

TS:   process.cwd()
来源：http://vjb.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://rwi.jianghu66.top

Go:   os.Getwd()
来源：http://lix.gaohongyu789.top

Ruby: Dir.pwd
来源：http://jio.cashguo.top

C#:   Directory.GetCurrentDirectory()
来源：http://tgm.yj20258.top

[M05] 设置退出码
来源：http://ahf.smart0.xyz

Py:   sys.exit(1)
来源：http://rrl.ivvv.top

PHP:  exit(1);
来源：http://vjl.hfpthk.cn

JS:   process.exit(1)
来源：http://leu.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://lor.jyoumei.cn

Java: System.exit(1)
来源：http://dud.redwolf501.top

Go:   os.Exit(1)
来源：http://ygi.tarul.cn

Ruby: exit 1
来源：http://kuu.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jiq.daxiang520.top

[M06] 向标准错误输出
来源：http://drx.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://knm.kuanghao11.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hki.jinghuilouyu.cn

JS:   console.error("err")
来源：http://wwp.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://bpj.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://nej.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lfi.yangfankeji.com

Ruby: warn "err"
来源：http://uuk.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://pld.sufxvd.cn

[M07] 判断是否为主入口
来源：http://kft.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://ddr.shanyushiyangtech.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qon.yj20258888.top

JS:   require.main === module
来源：http://jmo.guowangkeji.top

TS:   require.main === module
来源：http://nvf.shzxlz.cn

Java: public static void main(String[] args)
来源：http://bua.c1oappe.top

Go:   func main()
来源：http://zwz.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cyg.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://rbj.xuetiantiany.cn

[M08] 获取系统与运行时信息
来源：http://bjr.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://fto.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://zry.cdnleiting.top

JS:   process.platform;  process.version
来源：http://jqf.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://oez.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://afm.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xzc.sysykeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oig.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fgs.fehbvm.com

================================================================================
来源：http://jfn.jianghu66.top

N. 数据结构与算法
来源：http://xjy.sweek.top

================================================================================
来源：http://ski.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://gaa.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://ojj.birdmap.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fpj.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fwx.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hpg.smart0.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://zth.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://voq.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qii.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://qgx.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://cpn.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://lee.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aog.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vli.sweek.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xcg.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qdw.nwbrower.top

Go:   slices.Sort(arr)
来源：http://tqs.shuidangran.top

Ruby: arr.sort
来源：http://xyw.daxiang520.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://opy.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://wvv.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gao.aizwys.cn

PHP:  // 递归实现，或用 usort
来源：http://lpc.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vbp.yfazqb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://amv.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kag.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fdo.pengpengdd.cyou

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wvo.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kie.hammf.cn

[N04] 斐波那契数列
来源：http://bcd.zhengqikj.top


<!-- 参考信息 -->