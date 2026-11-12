代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dwx.hongshengwenyu.top

Ruby: Time.now + 7 * 86400
来源：http://leb.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://oab.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://qtg.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://pdo.birdmap.top

PHP:  $end->diff($start)->days;
来源：http://fhy.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gca.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qor.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://rqu.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://igu.tian-w.cn

Ruby: end - start                 # 返回秒数
来源：http://zuu.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://bey.aizwys.cn

[J07] 比较两个日期
来源：http://tso.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://sij.andypj.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yxv.shangyingyoupin.top

JS:   d1.getTime() < d2.getTime()
来源：http://htq.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://itg.yj202588.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mmv.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rat.yueranfly.top

Ruby: d1 < d2;  d1 == d2
来源：http://qtq.sufxvd.cn

C#:   d1 < d2;  d1 == d2
来源：http://wmi.zycfv.cn

[J08] 提取年月日与星期
来源：http://gup.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qyd.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tpj.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yzj.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hzr.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bjs.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jrl.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uzt.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nwz.cashguo.top

[J09] 时区处理
来源：http://twh.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wrk.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ftb.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ubn.shangyingyoupin.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cfh.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yqg.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ndz.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ubw.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jvl.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://pjn.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://lff.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yaq.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jga.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nme.jinghuilouyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wns.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rnp.zhoulong.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ukr.jianghu66.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cfm.guowangkeji.top

================================================================================
来源：http://qkt.jlsjyb.cn

K. JSON 与序列化
来源：http://abq.316326.xyz

================================================================================
来源：http://dow.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://egk.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ato.316326.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lli.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://oke.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://bkd.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://btn.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://tft.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hlf.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zit.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://pmk.sweek.top

Py:   json.loads(s)
来源：http://sgr.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mle.jinqigufen.top

JS:   JSON.parse(s)
来源：http://qvv.bbcook.cn

TS:   JSON.parse(s)
来源：http://bht.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kba.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://rap.ehwqpu.com

Ruby: JSON.parse(s)
来源：http://xbm.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://txp.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://jpr.fehbvm.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://opi.haohaochexian.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gxh.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pxg.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://enn.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gnc.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://guq.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lid.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tlm.yuxming.cn

[K04] 读取 JSON 文件
来源：http://cnq.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bfz.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://psw.hysaishi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lhc.zhongyouzk.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xvm.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gcr.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rmf.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ybq.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://brb.epnwcf.com

[K05] 深拷贝对象
来源：http://dtl.jinghuilouyu.cn

Py:   copy.deepcopy(obj)
来源：http://npw.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://gei.zhixingplan.top

JS:   structuredClone(obj)
来源：http://unv.havefunace.top

TS:   structuredClone(obj)
来源：http://cvp.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xbu.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://izo.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ijb.smart0.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://sat.sxryk.cn

[K06] 解析 URL 查询串
来源：http://lcs.chenlongwang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ihk.nanxuanxn.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rst.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pbi.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gjn.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pcf.vehdjk.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://mbk.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zbt.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://isd.bjfxy.top

[K07] 进制转换
来源：http://fcd.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qcy.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eob.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yzm.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://emm.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sun.yanxiufei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wyv.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fyu.jinyuanbaomall.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uzn.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://ufi.hnqzz.top

Py:   pickle.dumps(obj)
来源：http://smp.jianghu66.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jcv.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://jbr.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://jzj.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xzq.aibaodan.cn

Go:   encoding/gob
来源：http://ghr.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://mpp.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qfq.fktsv.cn

================================================================================
来源：http://gdt.ywan-chungtsiang.top

L. 网络请求
来源：http://yzo.jinyuanbaomall.cn

================================================================================
来源：http://svn.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://aog.fanxiaobao.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nag.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xus.smart0.xyz

JS:   await fetch(url)
来源：http://ksb.cucudq.cn

TS:   await fetch(url)
来源：http://ktn.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://brn.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://kbl.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wou.guannengcc.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bft.zhixingplan.top

[L02] 发送 POST JSON
来源：http://kyr.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yjv.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hrs.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://alr.shangyingyoupin.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://usf.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://smy.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tci.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qyw.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eaa.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://zvw.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://etn.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://feg.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oiz.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yxy.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xoc.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://owa.jiagoushi.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fbw.hammf.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cfl.daria6918.cn

[L04] 设置超时
来源：http://knc.pycfn.com

Py:   requests.get(url, timeout=5)
来源：http://arf.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sar.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gft.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bzl.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mzx.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ytd.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nhm.nanxuanxn.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cfg.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://cga.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qtu.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mlu.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xjd.ywan-chungtsiang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xff.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bjq.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://edf.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vhh.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gme.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://hcn.yongpay.top

Py:   resp.json()
来源：http://xeb.meibo888.top

PHP:  json_decode($body, true);
来源：http://uta.zhiwuduotai.top

JS:   await resp.json()
来源：http://eep.xziqi.cn

TS:   await resp.json()
来源：http://ygf.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fyn.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qzt.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://dfy.ywan-chungtsiang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ynx.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://sta.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://way.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vgl.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://bpf.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://avp.gzhubu.top

Java: resp.statusCode()
来源：http://ero.dianchejie.cn

Go:   resp.StatusCode
来源：http://ira.chenlongwang.top

Ruby: resp.code.to_i
来源：http://dgr.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://mnp.pycfn.com

[L08] 并发请求多个地址
来源：http://kss.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hwu.zhijiandao.cn

PHP:  curl_multi_init() 系列
来源：http://zhz.yonumen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yqp.zhongyouzk.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zqp.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ibe.9152youxi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tnw.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gjv.fanxiaobao.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ehn.dianchejie.cn

================================================================================
来源：http://tcp.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://zus.quarkkingdee.top

================================================================================
来源：http://acn.shzxlz.cn

[M01] 读取命令行参数
来源：http://vgx.hywenlv.cn

Py:   sys.argv[1:]
来源：http://qgx.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://coc.andypj.xyz

JS:   process.argv.slice(2)
来源：http://rkn.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://dzf.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://jtu.chenjidiqi.icu

Go:   os.Args[1:]
来源：http://uud.vehdjk.com

Ruby: ARGV
来源：http://gjf.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://bnb.chenzaomai.com

[M02] 读取环境变量
来源：http://xnx.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://kxq.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eau.hywenlv.cn

JS:   process.env.HOME
来源：http://ezs.jqgufenzy.top

TS:   process.env.HOME
来源：http://fky.nanxuanxn.top

Java: System.getenv("HOME")
来源：http://smb.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://txk.fktsv.cn

Ruby: ENV["HOME"]
来源：http://mko.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://omv.aibaodan.cn

[M03] 执行外部命令
来源：http://ijr.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tal.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gqu.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tlr.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xnf.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tkc.ydzc1.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jxr.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bkd.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://fru.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://cne.zhijiandao.cn

Py:   os.getcwd()
来源：http://gpw.ydjk.org.cn

PHP:  getcwd();
来源：http://ssb.cdnleiting.top

JS:   process.cwd()
来源：http://ogf.sjlbkw.cn

TS:   process.cwd()
来源：http://kwb.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://pjj.xuanzx.com

Go:   os.Getwd()
来源：http://zpw.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://cvy.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uyk.jqgufenzy.top

[M05] 设置退出码
来源：http://imd.hnxiangtu.top

Py:   sys.exit(1)
来源：http://vak.birdmap.top

PHP:  exit(1);
来源：http://vhv.cheryme.top

JS:   process.exit(1)
来源：http://fke.ivvv.top

TS:   process.exit(1)
来源：http://lix.fengsongda.top

Java: System.exit(1)
来源：http://wsu.gotoacloud.top

Go:   os.Exit(1)
来源：http://pcp.sxryk.cn

Ruby: exit 1
来源：http://xgg.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://acu.svipenyu.cn

[M06] 向标准错误输出
来源：http://fut.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://kjz.xuanzx.com

PHP:  fwrite(STDERR, "err\n");
来源：http://udf.andypj.xyz

JS:   console.error("err")
来源：http://uez.shangyingyoupin.top

TS:   console.error("err")
来源：http://sud.guowangkeji.top

Java: System.err.println("err")
来源：http://qpt.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zyg.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://jps.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://jpb.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://dkt.mhx1999.top

Py:   if __name__ == "__main__":
来源：http://ayg.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xmx.fanxiaobao.xyz

JS:   require.main === module
来源：http://lbp.zhijiandao.cn

TS:   require.main === module
来源：http://puy.yvedp.cn

Java: public static void main(String[] args)
来源：http://dwf.nanxinkj.top

Go:   func main()
来源：http://dgp.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://onr.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://ptr.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://avc.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://dht.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://gth.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://nhd.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://xzv.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xkd.aizwys.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tfc.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rbu.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://frw.jqgfzy.top

================================================================================
来源：http://zlu.jinyuanbaomall.cn

N. 数据结构与算法
来源：http://ahd.9152youxi.cn

================================================================================
来源：http://dsx.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://ymj.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://uec.snrcjt.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qfa.yvedp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mpk.tian-w.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jqu.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lbw.guannengcc.top

Go:   sort.SearchInts(arr, x)
来源：http://kdb.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lzs.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pqu.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://mdw.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://bxg.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pny.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wmi.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://mqb.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ldb.yonumen.top

Go:   slices.Sort(arr)
来源：http://mdv.daria6918.cn

Ruby: arr.sort
来源：http://plc.tanke756.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yaa.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://uyf.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://utx.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://ccs.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rla.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://abl.uphjek.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sqk.nanxuanxn.top


<!-- 参考信息 -->