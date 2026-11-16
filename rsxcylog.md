代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://bvw.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zuy.pycfn.com

JS:   s.split(/\s*,\s*/)
来源：http://rsh.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://zjd.hammf.cn

Java: s.split("\\s*,\\s*")
来源：http://rxu.yj20258888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pbf.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://bdu.haohaochexian.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ato.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uwc.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://twz.vqdsnc.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nne.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://omi.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dlm.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fvv.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gml.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ual.chenzaomai.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zkj.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://nnm.uphjek.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bhx.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tmc.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uxd.daxiang520.top

TS:   /error/gim
来源：http://rzb.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cmj.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kqf.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://rsn.hesvh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zst.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://pxh.jiagoushi.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://igr.jqgfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pci.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://npv.zhengqikj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iaf.yueranfly.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://luo.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jor.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://smy.zhiwuduotai.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cya.hammf.cn

================================================================================
来源：http://lws.jinyuanbaomall.cn

J. 日期与时间
来源：http://nwc.yfazqb.com

================================================================================
来源：http://lso.yfazqb.com

[J01] 获取当前时间
来源：http://ctt.ehwqpu.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://wlx.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uff.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://hfh.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://xhd.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rvv.fanxiaobao.xyz

Go:   time.Now()
来源：http://woy.hfpthk.cn

Ruby: Time.now
来源：http://pfp.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://atm.jyoumei.cn

[J02] 格式化输出
来源：http://qll.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jqa.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cyc.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vai.hnqzz.top

TS:   d.toISOString()
来源：http://vlr.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gaa.aibaodan.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lij.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iim.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fys.nwbrower.top

[J03] 字符串解析为日期
来源：http://vvz.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vfe.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qju.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://exx.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://ayw.redwolf501.top

Java: LocalDate.parse("2024-01-02")
来源：http://dzk.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ygw.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://lyn.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jxy.yueranfly.top

[J04] 时间戳与日期互转
来源：http://jxs.andypj.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nwd.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rdm.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mke.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://uqv.cqqwz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eab.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://flf.yfazqb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pry.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vkd.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://woe.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://gge.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nap.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fpz.havefunace.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://riq.hfpthk.cn

Java: LocalDate.now().plusDays(7)
来源：http://xnj.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bve.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://uru.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://wjl.cheryme.top

[J06] 计算两时间之差
来源：http://xjc.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://uxh.svipenyu.cn

PHP:  $end->diff($start)->days;
来源：http://cnh.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://juz.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ech.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://zkg.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://auk.guowangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://ede.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://wbf.zhijiandao.cn

[J07] 比较两个日期
来源：http://one.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://dwy.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://njy.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://wvv.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mmm.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ujg.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gqj.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://mgr.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://dqh.chenlongwang.top

[J08] 提取年月日与星期
来源：http://wlp.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ygu.yfazqb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fyv.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jcz.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pzj.vehdjk.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hvp.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pnm.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ysv.ybcxt.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yfy.shzxlz.cn

[J09] 时区处理
来源：http://rev.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://orl.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hsw.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kxe.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wpy.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xgo.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vhd.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gor.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kap.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://dfv.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hve.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mxe.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://quw.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hjn.fktsv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jkt.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pgv.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mhr.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dok.vehdjk.com

================================================================================
来源：http://oba.ivvv.top

K. JSON 与序列化
来源：http://klp.cdnleiting.top

================================================================================
来源：http://jkh.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://bjq.gzhubu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://psb.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gjs.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://nhi.tarul.cn

TS:   JSON.stringify(obj)
来源：http://mwt.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://isp.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://eaz.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ofn.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dcy.tarul.cn

[K02] JSON 字符串转对象
来源：http://fae.guowangkeji.top

Py:   json.loads(s)
来源：http://qwj.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uih.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://rwa.dashuyun.cn

TS:   JSON.parse(s)
来源：http://cis.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qmw.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://xoy.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://clo.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iwj.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://zvw.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rkf.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ohw.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xhe.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ofe.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qfr.xziqi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kmj.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://eaj.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tzx.bjfxy.top

[K04] 读取 JSON 文件
来源：http://scx.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cia.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dvz.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bhr.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://npk.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bpk.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lcd.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xrp.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qjx.vqdsnc.cn

[K05] 深拷贝对象
来源：http://ogt.0kj1m.cn

Py:   copy.deepcopy(obj)
来源：http://zpc.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://owp.fzhhl.top

JS:   structuredClone(obj)
来源：http://bmu.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://lot.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nqf.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xpw.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ghc.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zrn.bbcook.cn

[K06] 解析 URL 查询串
来源：http://twv.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rgy.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aij.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://izj.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://anj.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vbk.jinghuilouyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://awz.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pls.epnwcf.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ktr.ybcxt.top

[K07] 进制转换
来源：http://xsu.xingfuxueyuan.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://egm.wangshuangyany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hhl.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ris.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ilr.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xxb.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zme.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zxt.jinyuanbaomall.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ory.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://lml.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://dlg.zycfv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ltg.0kj1m.cn

JS:   v8.serialize(obj)        // Node
来源：http://rdi.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://mok.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tkj.ydjk.org.cn

Go:   encoding/gob
来源：http://ktp.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://etc.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pqp.yj20258888.top

================================================================================
来源：http://mca.yonumen.top

L. 网络请求
来源：http://mvb.pycfn.com

================================================================================
来源：http://frj.fzhhl.top

[L01] 发送 GET 请求
来源：http://cum.tarul.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mri.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ahg.hesvh.cn

JS:   await fetch(url)
来源：http://jud.pengpengdd.cyou

TS:   await fetch(url)
来源：http://yfe.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qjt.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://tgt.meibo888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wbu.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ohr.ydzc1.top

[L02] 发送 POST JSON
来源：http://quk.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://kda.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fod.mhx1999.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mpd.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tds.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wtu.jiagoushi.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oig.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zul.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fiy.hywenlv.cn

[L03] 设置自定义请求头
来源：http://kwd.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qvy.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mic.pengpengdd.cyou

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ece.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wxw.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mjz.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rmc.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blq.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wes.shzxlz.cn

[L04] 设置超时
来源：http://rwl.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://khl.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ttl.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ydy.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fry.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ojd.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xzu.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ckf.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wbw.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://lox.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ihk.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hsr.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eyp.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jtk.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vvx.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pcx.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://utf.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://trc.daria6918.cn

[L06] 解析响应为 JSON
来源：http://hdh.cucudq.cn

Py:   resp.json()
来源：http://ive.redwolf501.top

PHP:  json_decode($body, true);
来源：http://gbq.hysaishi.cn

JS:   await resp.json()
来源：http://nks.shuidangran.top

TS:   await resp.json()
来源：http://llm.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oby.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://efk.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://msh.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://env.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://tvn.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fcl.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wii.0kj1m.cn

JS:   resp.ok;  resp.status
来源：http://czn.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://zua.mhx1999.top

Java: resp.statusCode()
来源：http://hnn.52xcode.cn

Go:   resp.StatusCode
来源：http://qow.vqdsnc.cn

Ruby: resp.code.to_i
来源：http://zpe.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://wxb.yfazqb.com

[L08] 并发请求多个地址
来源：http://iqp.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://igw.zdbjq.cn

PHP:  curl_multi_init() 系列
来源：http://bdj.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kxu.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zqc.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wzm.nanxinkj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rwk.hywenlv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tcz.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://foq.yonumen.top

================================================================================
来源：http://wlq.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://fzi.uphjek.com

================================================================================
来源：http://lox.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://iln.jiagoushi.top

Py:   sys.argv[1:]
来源：http://nlu.zhaomingkeji.xyz

PHP:  $argv;  $argc;
来源：http://hsu.fehbvm.com

JS:   process.argv.slice(2)
来源：http://uho.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://zad.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://sbv.dianchejie.cn

Go:   os.Args[1:]
来源：http://uta.nanxinkj.top

Ruby: ARGV
来源：http://auj.dashuyun.cn

C#:   args 数组（Main 方法参数）
来源：http://jwc.chenlongwang.top

[M02] 读取环境变量
来源：http://oom.shanyushiyangtech.top

Py:   os.environ.get("HOME")
来源：http://inu.ydzc1.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wjl.yueranfly.top

JS:   process.env.HOME
来源：http://fzw.jinghuilouyu.cn

TS:   process.env.HOME
来源：http://zqv.yuxming.cn

Java: System.getenv("HOME")
来源：http://iju.jyoumei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tkw.cucudq.cn

Ruby: ENV["HOME"]
来源：http://uuf.yuxming.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kqi.andypj.xyz

[M03] 执行外部命令
来源：http://xsf.hammf.cn


<!-- 参考信息 -->