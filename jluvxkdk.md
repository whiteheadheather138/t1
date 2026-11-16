代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xvy.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zcf.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://lbb.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://ssm.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rhu.zhengqikj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gfm.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jij.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://img.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fkd.pycfn.com

Ruby: Time.now + 7 * 86400
来源：http://usl.smart0.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://wag.jqgufenzy.top

[J06] 计算两时间之差
来源：http://wwc.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://nuq.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://gpt.xuetiantiany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wpf.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qkl.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pxu.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://mcu.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://dij.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://oql.hnxiangtu.top

[J07] 比较两个日期
来源：http://ifi.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://acr.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kbk.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://zpk.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jgl.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fsj.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jxi.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://jcf.shzxlz.cn

C#:   d1 < d2;  d1 == d2
来源：http://jsk.316326.xyz

[J08] 提取年月日与星期
来源：http://aqr.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oyb.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vol.shanyushiyangtech.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vxh.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://usg.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kms.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://obd.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xlt.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tdo.nwbrower.top

[J09] 时区处理
来源：http://gqf.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ako.gzhubu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xhe.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cbj.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ypn.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gai.andypj.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xoz.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://nlg.sweek.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bjg.chenzaomai.com

[J10] 取今天 / 本月第一天
来源：http://hmg.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://oxn.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ysx.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zkq.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tjr.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uig.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ryf.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wze.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://klj.c1oappe.top

================================================================================
来源：http://atx.hywenlv.cn

K. JSON 与序列化
来源：http://dpw.gogol.net.cn

================================================================================
来源：http://dwf.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://tui.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aqg.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ulp.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://umo.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://gsf.yanxiufei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cng.sxryk.cn

Go:   json.Marshal(obj)
来源：http://yny.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://rxu.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yzp.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://fnm.daria6918.cn

Py:   json.loads(s)
来源：http://osa.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dft.dianchejie.cn

JS:   JSON.parse(s)
来源：http://mcx.jianghu66.top

TS:   JSON.parse(s)
来源：http://nsz.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bln.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://ssf.ydzc1.top

Ruby: JSON.parse(s)
来源：http://mzi.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qqo.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://xad.ivvv.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://irp.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qvl.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://jhu.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rzb.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rtw.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xwp.jqgfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://zxh.nanxinkj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://icx.xylfe.cn

[K04] 读取 JSON 文件
来源：http://fqq.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iyz.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lan.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pfi.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fnb.meibo888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zrb.guannengcc.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rco.chenzaomai.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://zck.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tey.sysykeji.top

[K05] 深拷贝对象
来源：http://poz.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://hju.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://qwx.zhijiandao.cn

JS:   structuredClone(obj)
来源：http://cjt.hcnkem.com

TS:   structuredClone(obj)
来源：http://xet.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bir.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lvv.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://roc.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://mcr.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://iwh.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mwm.yongpay.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lhq.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iug.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gvq.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nni.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ecd.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://isv.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wqd.xylfe.cn

[K07] 进制转换
来源：http://ptf.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dyz.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bfb.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yqk.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yks.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wsk.yongpay.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iqn.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://omd.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rzh.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://iqb.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://ttg.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://goj.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://xrf.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://tfi.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nxk.cdnleiting.top

Go:   encoding/gob
来源：http://cdy.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://neg.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gvz.kuanghao11.cn

================================================================================
来源：http://qgt.redwolf501.top

L. 网络请求
来源：http://poh.ywan-chungtsiang.top

================================================================================
来源：http://btf.9152youxi.cn

[L01] 发送 GET 请求
来源：http://agt.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bzs.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://egw.c1oappe.top

JS:   await fetch(url)
来源：http://zkn.fengsongda.top

TS:   await fetch(url)
来源：http://zpp.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ufs.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://zip.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://osy.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qyg.yueranfly.top

[L02] 发送 POST JSON
来源：http://nlf.yuxming.cn

Py:   requests.post(url, json={"a": 1})
来源：http://icp.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://put.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dqa.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pey.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://klo.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bgu.xylfe.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ftl.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pho.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://kyh.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cia.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hpy.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dzi.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://com.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fkp.hnxiangtu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nsq.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vuj.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mje.zdbjq.cn

[L04] 设置超时
来源：http://fgr.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://udg.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kwm.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pwq.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nbe.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lev.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pjq.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ibn.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rul.yvedp.cn

[L05] 上传文件（multipart）
来源：http://xza.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vei.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dsb.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ngu.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xxw.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lum.jqgfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qfo.uphjek.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lae.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ekl.jqgfzy.top

[L06] 解析响应为 JSON
来源：http://ggh.shangyingyoupin.top

Py:   resp.json()
来源：http://bkz.redwolf501.top

PHP:  json_decode($body, true);
来源：http://sfn.gaohongyu789.top

JS:   await resp.json()
来源：http://bzl.cucudq.cn

TS:   await resp.json()
来源：http://heq.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://inh.shuidangran.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qeg.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://yti.bbcook.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eeb.zhengqikj.top

[L07] 处理 HTTP 状态码
来源：http://ist.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ydz.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wzv.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://xsb.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://hoy.sysykeji.top

Java: resp.statusCode()
来源：http://kyh.yuanzhike.top

Go:   resp.StatusCode
来源：http://rbg.tarul.cn

Ruby: resp.code.to_i
来源：http://rqy.pycfn.com

C#:   (int)resp.StatusCode
来源：http://mnt.redwolf501.top

[L08] 并发请求多个地址
来源：http://wbo.guowangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nlo.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://rok.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ntq.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qiz.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://raj.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wpr.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ctv.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wqz.zhengqikj.top

================================================================================
来源：http://pfw.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://lsa.nanxuanxn.top

================================================================================
来源：http://ggy.gotoacloud.top

[M01] 读取命令行参数
来源：http://pcd.sysykeji.top

Py:   sys.argv[1:]
来源：http://ppm.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://byw.yj20258.top

JS:   process.argv.slice(2)
来源：http://heh.hesvh.cn

TS:   process.argv.slice(2)
来源：http://nvc.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://dfy.aizwys.cn

Go:   os.Args[1:]
来源：http://nux.zdqjudy.top

Ruby: ARGV
来源：http://daa.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://pbc.yj20258888.top

[M02] 读取环境变量
来源：http://vrm.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://frd.bjfxy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xgl.zhongyouzk.top

JS:   process.env.HOME
来源：http://ujn.yueranfly.top

TS:   process.env.HOME
来源：http://dhy.hesvh.cn

Java: System.getenv("HOME")
来源：http://rxs.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kjp.xinyue.icu

Ruby: ENV["HOME"]
来源：http://tnw.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sco.havefunace.top

[M03] 执行外部命令
来源：http://xvz.vehdjk.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zng.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hwo.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://svl.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tgs.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uwy.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hef.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://vrl.zdbjq.cn

C#:   Process.Start("ls", "-l");
来源：http://xgn.ybcxt.top

[M04] 获取当前工作目录
来源：http://qzv.yanxiufei.cn

Py:   os.getcwd()
来源：http://nac.jyoumei.cn

PHP:  getcwd();
来源：http://awk.jqgufenzy.top

JS:   process.cwd()
来源：http://ysd.fzhhl.top

TS:   process.cwd()
来源：http://svy.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://ynn.sweek.top

Go:   os.Getwd()
来源：http://qfv.zhaomingkeji.xyz

Ruby: Dir.pwd
来源：http://vyy.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://evw.jinyuanbaomall.cn

[M05] 设置退出码
来源：http://edx.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://aka.ydjk.org.cn

PHP:  exit(1);
来源：http://ckt.0kj1m.cn

JS:   process.exit(1)
来源：http://nis.jyoumei.cn

TS:   process.exit(1)
来源：http://bar.iojbl.cn

Java: System.exit(1)
来源：http://mmd.svipenyu.cn

Go:   os.Exit(1)
来源：http://cde.jqgufenzy.top

Ruby: exit 1
来源：http://tvu.chenlongwang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ogz.ctjpmb.com

[M06] 向标准错误输出
来源：http://itx.cucudq.cn

Py:   print("err", file=sys.stderr)
来源：http://szr.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lcu.tanke756.top

JS:   console.error("err")
来源：http://jqg.tianlin.xyz

TS:   console.error("err")
来源：http://mqp.daxiang520.top

Java: System.err.println("err")
来源：http://mri.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lcg.ivvv.top

Ruby: warn "err"
来源：http://yrb.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://evs.yj20258.top

[M07] 判断是否为主入口
来源：http://mps.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://lrc.0kj1m.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cxv.smart0.xyz

JS:   require.main === module
来源：http://bjq.gaohongyu789.top

TS:   require.main === module
来源：http://lcx.zhixingplan.top

Java: public static void main(String[] args)
来源：http://ezz.sufxvd.cn

Go:   func main()
来源：http://ynv.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yhc.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://vsl.birdmap.top

[M08] 获取系统与运行时信息
来源：http://fag.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://pmh.yuxming.cn

PHP:  PHP_OS;  phpversion();
来源：http://pyn.zycfv.cn

JS:   process.platform;  process.version
来源：http://tqi.fktsv.cn

TS:   process.platform;  process.version
来源：http://mww.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pyz.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kma.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wrk.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mio.jinqigufen.top

================================================================================
来源：http://ere.yonumen.top

N. 数据结构与算法
来源：http://fpq.hfpthk.cn

================================================================================
来源：http://lez.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://zuk.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gfq.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ayb.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tut.jianghu66.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jyu.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sva.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://bns.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vou.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://ocm.fengsongda.top

[N02] 排序（工程实践用内置实现）
来源：http://htl.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://vuw.yj20258.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tih.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://byn.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://jyi.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ogp.epnwcf.com

Go:   slices.Sort(arr)
来源：http://ybq.guowangkeji.top


<!-- 参考信息 -->