代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://efa.tianlin.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hhb.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uxp.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://hbr.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mql.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://zbt.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hcq.zhongyouzk.top

[J06] 计算两时间之差
来源：http://qdw.tarul.cn

Py:   (end - start).total_seconds()
来源：http://yuu.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://eus.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cuu.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vng.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://ivu.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://ufa.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://yej.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://qjz.yongpay.top

[J07] 比较两个日期
来源：http://swg.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://xuc.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://orx.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fty.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://awl.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xjw.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bxj.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kqw.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://kzi.smart0.xyz

[J08] 提取年月日与星期
来源：http://wng.daria6918.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tob.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wnv.ydzc1.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://huw.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sgx.feifeiyinyue.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mzk.chenlongwang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bom.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jsc.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vgl.cdnleiting.top

[J09] 时区处理
来源：http://rld.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ixa.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://plm.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rhj.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://axx.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://woo.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qmc.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mro.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gjn.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://yqt.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ork.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ezi.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://htq.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xyu.quarkkingdee.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qsj.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://esz.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gpo.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ylv.svipenyu.cn

================================================================================
来源：http://cwx.yfazqb.com

K. JSON 与序列化
来源：http://kfh.kuanghao11.cn

================================================================================
来源：http://efb.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://tib.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qwl.jianghu66.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qyn.xingfuxueyuan.xyz

JS:   JSON.stringify(obj)
来源：http://xqv.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://ucg.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gad.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://acn.redwolf501.top

Ruby: obj.to_json                                     // require "json"
来源：http://ipb.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zkl.epnwcf.com

[K02] JSON 字符串转对象
来源：http://spr.xuanzx.com

Py:   json.loads(s)
来源：http://sqv.yj202588.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qiy.fehbvm.com

JS:   JSON.parse(s)
来源：http://jyp.birdmap.top

TS:   JSON.parse(s)
来源：http://qnm.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oxu.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://thi.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://wwf.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ngd.tianlin.xyz

[K03] JSON 美化输出（带缩进）
来源：http://mgm.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vcv.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zfw.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://quq.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nok.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xps.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sxj.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://iep.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ziu.nwbrower.top

[K04] 读取 JSON 文件
来源：http://acz.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://siy.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lfv.cheryme.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://prr.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kmw.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uvq.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://awu.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ktp.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fwi.zycfv.cn

[K05] 深拷贝对象
来源：http://xxu.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://fen.52xcode.cn

PHP:  unserialize(serialize($obj));
来源：http://xke.daxiang520.top

JS:   structuredClone(obj)
来源：http://srx.guannengcc.top

TS:   structuredClone(obj)
来源：http://njy.chenlongwang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://chj.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cna.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yne.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ykw.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://hfh.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hql.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nwf.dashuyun.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rge.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dgz.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://brl.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sdv.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://way.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mlf.haohaochexian.top

[K07] 进制转换
来源：http://ner.yuxming.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ynl.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hfz.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ohh.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ovf.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://izh.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ogt.hcnkem.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nny.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tri.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://lei.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://aia.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eya.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://mod.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://nco.sufxvd.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://omi.sweek.top

Go:   encoding/gob
来源：http://vbj.jinqigfzy.top

Ruby: Marshal.dump(obj)
来源：http://nkh.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ydu.zycfv.cn

================================================================================
来源：http://qpm.chenlongwang.top

L. 网络请求
来源：http://mnn.zhoulong.xyz

================================================================================
来源：http://pgv.yuxming.cn

[L01] 发送 GET 请求
来源：http://nvb.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xdx.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nyd.nwbrower.top

JS:   await fetch(url)
来源：http://hxc.jlsjyb.cn

TS:   await fetch(url)
来源：http://juj.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://toh.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://lsj.shuidangran.top

Ruby: Net::HTTP.get(URI(url))
来源：http://odo.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://scd.hfpthk.cn

[L02] 发送 POST JSON
来源：http://dzi.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://qip.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hnd.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rzs.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dmw.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jxy.ydjk.org.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lrh.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pdl.chenlongwang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dyc.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://ggk.fengsongda.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pnm.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rdw.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sgr.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fjr.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jjj.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tye.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yth.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fwy.fengsongda.top

[L04] 设置超时
来源：http://qbz.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://yew.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wqe.wangdashe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xsx.yj202588.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://enu.ctjpmb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iwn.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wla.zhixingplan.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tsj.smart0.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gjr.wangshuangyany.cn

[L05] 上传文件（multipart）
来源：http://loa.hysaishi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dtt.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aia.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pew.zhijiandao.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://whg.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oxr.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uhv.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iby.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kwv.shanyushiyangkeji.top

[L06] 解析响应为 JSON
来源：http://utm.nanxinkj.top

Py:   resp.json()
来源：http://ahr.redwolf501.top

PHP:  json_decode($body, true);
来源：http://svb.zhongyouzk.top

JS:   await resp.json()
来源：http://uca.ivvv.top

TS:   await resp.json()
来源：http://qwh.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jag.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wfm.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://ndg.hysaishi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://biq.xinyue.icu

[L07] 处理 HTTP 状态码
来源：http://yxg.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wnj.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vma.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://yvr.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://nfk.jinyuanbaomall.cn

Java: resp.statusCode()
来源：http://abw.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://ttd.jqgfzy.top

Ruby: resp.code.to_i
来源：http://vuv.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://bbr.vehdjk.com

[L08] 并发请求多个地址
来源：http://ser.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://svx.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://jhe.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ghf.zhijiandao.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pcw.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://htg.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ujj.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nve.zhengqikj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vbg.hammf.cn

================================================================================
来源：http://lgy.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://ygo.zdbjq.cn

================================================================================
来源：http://aif.yonumen.top

[M01] 读取命令行参数
来源：http://zcb.xinyue.icu

Py:   sys.argv[1:]
来源：http://hnh.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://ire.daxiang520.top

JS:   process.argv.slice(2)
来源：http://jkr.epnwcf.com

TS:   process.argv.slice(2)
来源：http://pnb.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://eji.jinqigfzy.top

Go:   os.Args[1:]
来源：http://xxk.yj202588.top

Ruby: ARGV
来源：http://fgk.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://wmc.cdnleiting.top

[M02] 读取环境变量
来源：http://nvf.jinqigfzy.top

Py:   os.environ.get("HOME")
来源：http://qah.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tkv.daria6918.cn

JS:   process.env.HOME
来源：http://tmi.fktsv.cn

TS:   process.env.HOME
来源：http://tqb.chenjidiqi.icu

Java: System.getenv("HOME")
来源：http://rvb.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pzv.yuanzhike.top

Ruby: ENV["HOME"]
来源：http://zrl.hammf.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nga.yonumen.top

[M03] 执行外部命令
来源：http://lxr.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gpy.gaohongyu789.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ynt.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://amv.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jrh.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gub.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://jyr.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aer.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://pry.havefunace.top

[M04] 获取当前工作目录
来源：http://ybu.dashuyun.cn

Py:   os.getcwd()
来源：http://bll.nanxinkj.top

PHP:  getcwd();
来源：http://dxo.chenjidiqi.icu

JS:   process.cwd()
来源：http://ubz.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://xwh.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://trp.yueranfly.top

Go:   os.Getwd()
来源：http://kmi.svipenyu.cn

Ruby: Dir.pwd
来源：http://aik.sjlbkw.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bba.hesvh.cn

[M05] 设置退出码
来源：http://pgx.kuanghao11.cn

Py:   sys.exit(1)
来源：http://cyb.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://igg.feifeiyinyue.top

JS:   process.exit(1)
来源：http://qgn.svipenyu.cn

TS:   process.exit(1)
来源：http://uhr.guowangkeji.top

Java: System.exit(1)
来源：http://thl.kuanghao11.cn

Go:   os.Exit(1)
来源：http://imy.pycfn.com

Ruby: exit 1
来源：http://akk.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fmk.wangdashe.top

[M06] 向标准错误输出
来源：http://oox.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://qnm.hcnkem.com

PHP:  fwrite(STDERR, "err\n");
来源：http://zwq.andypj.xyz

JS:   console.error("err")
来源：http://fyf.sufxvd.cn

TS:   console.error("err")
来源：http://oed.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://wqy.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hdg.yj20258888.top

Ruby: warn "err"
来源：http://jaf.xylfe.cn

C#:   Console.Error.WriteLine("err")
来源：http://syt.chenzaomai.com

[M07] 判断是否为主入口
来源：http://pwh.tanke756.top

Py:   if __name__ == "__main__":
来源：http://adz.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mef.jianghu66.top

JS:   require.main === module
来源：http://vbu.9152youxi.cn

TS:   require.main === module
来源：http://kpk.epnwcf.com

Java: public static void main(String[] args)
来源：http://mlt.guowangkeji.top

Go:   func main()
来源：http://lvt.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jbn.ydzc1.top

C#:   static void Main(string[] args)
来源：http://dxh.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://wqg.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://ajb.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://rws.0kj1m.cn

JS:   process.platform;  process.version
来源：http://bfx.chenjidiqi.icu

TS:   process.platform;  process.version
来源：http://sxx.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://knh.shzxlz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zda.fzhhl.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pys.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tnx.redwolf501.top

================================================================================
来源：http://ubg.fzhhl.top

N. 数据结构与算法
来源：http://ibb.redwolf501.top

================================================================================
来源：http://xpi.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://ulf.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kkv.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bhm.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cfw.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ufs.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tth.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://imx.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://sig.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://rtk.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://dbv.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://jdq.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uys.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bmy.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://hix.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hgr.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://rte.xziqi.cn

Ruby: arr.sort
来源：http://vhb.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ytj.cqqwz.cn

[N03] 快速排序（分治示例）
来源：http://nvh.yonumen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qux.zhengqikj.top


<!-- 参考信息 -->