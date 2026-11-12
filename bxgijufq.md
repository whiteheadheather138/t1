代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://luj.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hut.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dry.yj20258.top

[I05] 按正则拆分
来源：http://ytk.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ljf.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fbn.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://nox.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://ese.xinyue.icu

Java: s.split("\\s*,\\s*")
来源：http://chs.fehbvm.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://krx.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cel.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uas.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iyf.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://opb.sweek.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cuk.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ruf.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dcz.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xvp.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gzs.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pyl.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pqb.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://xxs.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fzw.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uzs.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ewk.yj202588.top

TS:   /error/gim
来源：http://mth.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://civ.svipenyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ucu.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://xps.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ngf.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://akh.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zjc.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gri.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pal.jianghu66.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wsq.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://twf.yongpay.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bxo.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vsk.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vcu.yuxming.cn

================================================================================
来源：http://yxf.shangyingyoupin.top

J. 日期与时间
来源：http://xfd.ywan-chungtsiang.top

================================================================================
来源：http://pka.gogol.net.cn

[J01] 获取当前时间
来源：http://vcd.jinghuilouyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://moh.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hkb.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://lrq.0kj1m.cn

TS:   new Date();  Date.now()
来源：http://ybf.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://afl.jinyuanbaomall.cn

Go:   time.Now()
来源：http://wfd.tanke756.top

Ruby: Time.now
来源：http://ean.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rdn.pengpengdd.cyou

[J02] 格式化输出
来源：http://gjw.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://upm.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qty.meibo888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://esv.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://qjg.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://suv.jinyuanbaomall.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://keo.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aue.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zyx.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://uam.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ibu.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ejh.zhoulong.xyz

JS:   new Date("2024-01-02")
来源：http://ofh.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://ydv.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://wxi.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://scw.fanxiaobao.xyz

Ruby: Date.parse("2024-01-02")
来源：http://qje.ywan-chungtsiang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://phc.chenzaomai.com

[J04] 时间戳与日期互转
来源：http://elt.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zsk.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ztz.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nsa.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lho.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vso.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bgo.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mwz.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eri.jinghuilouyu.cn

[J05] 时间加减（加 7 天）
来源：http://ret.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://zia.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://mao.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ozi.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rto.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://jpq.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mkf.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://wqb.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://yqc.nanxinkj.top

[J06] 计算两时间之差
来源：http://xxi.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://ifc.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://qxu.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mbe.guannengcc.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vpt.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://mxr.daxiang520.top

Go:   end.Sub(start).Hours()
来源：http://une.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://unj.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://tcy.andypj.xyz

[J07] 比较两个日期
来源：http://jag.zycfv.cn

Py:   d1 < d2;  d1 == d2
来源：http://yca.wangshuangyany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qmq.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://htn.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wxz.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ypo.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://auc.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fyi.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://xlt.jianghu66.top

[J08] 提取年月日与星期
来源：http://myf.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cdr.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mkc.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://snj.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ljs.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://taf.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://exm.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ruv.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://reg.yuanzhike.top

[J09] 时区处理
来源：http://sqq.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://brw.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wuz.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://emc.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dxa.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hot.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dcq.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://whs.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://htq.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://pyc.jinqigufen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fxj.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bdn.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nvv.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vmt.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dpy.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rzl.hammf.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://izc.ehwqpu.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qfz.uphjek.com

================================================================================
来源：http://xwk.xinyue.icu

K. JSON 与序列化
来源：http://wlj.chenlongwang.top

================================================================================
来源：http://mqb.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://lxn.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xqy.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aos.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://dkm.hammf.cn

TS:   JSON.stringify(obj)
来源：http://byv.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://myx.tarul.cn

Go:   json.Marshal(obj)
来源：http://qox.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://mea.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ebd.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://kij.jqgfzy.top

Py:   json.loads(s)
来源：http://hlr.mhx1999.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tjj.guowangkeji.top

JS:   JSON.parse(s)
来源：http://lle.cucudq.cn

TS:   JSON.parse(s)
来源：http://rab.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zpr.quarkkingdee.top

Go:   json.Unmarshal(data, &v)
来源：http://qnl.yuxming.cn

Ruby: JSON.parse(s)
来源：http://fei.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mav.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://mqz.yongpay.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dkq.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ktt.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sqh.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fsa.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xpv.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wzl.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://zdm.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nyb.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://hjk.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xts.0kj1m.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qvp.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tnq.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ljq.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yut.ivvv.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fbs.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://spn.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rul.sweek.top

[K05] 深拷贝对象
来源：http://zjb.havefunace.top

Py:   copy.deepcopy(obj)
来源：http://zhc.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://jhi.sysykeji.top

JS:   structuredClone(obj)
来源：http://dkw.zdbjq.cn

TS:   structuredClone(obj)
来源：http://rzt.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bfl.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kpm.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oil.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hva.xinyue.icu

[K06] 解析 URL 查询串
来源：http://tdk.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qly.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nrt.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ywe.zhongyouzk.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xnp.zhixingplan.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yoa.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wep.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bqf.zhaomingkeji.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://grb.c1oappe.top

[K07] 进制转换
来源：http://mig.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jfr.xingfuxueyuan.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://phs.sysykeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ccu.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cxe.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iaa.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xaj.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dgo.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qfe.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://bgu.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://wwx.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pzf.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://ywu.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://dth.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hsg.yfazqb.com

Go:   encoding/gob
来源：http://ose.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://wix.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dcu.yj202588.top

================================================================================
来源：http://yxp.zhiwuduotai.top

L. 网络请求
来源：http://czn.redwolf501.top

================================================================================
来源：http://weu.yj202588.top

[L01] 发送 GET 请求
来源：http://oig.haohaochexian.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jgm.yuxming.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xxx.xuanzx.com

JS:   await fetch(url)
来源：http://krc.hfpthk.cn

TS:   await fetch(url)
来源：http://rdy.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gan.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://mfy.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://kzn.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://brr.guannengcc.top

[L02] 发送 POST JSON
来源：http://qno.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://usp.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qgh.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mvi.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rsf.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jss.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qqd.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fsy.guannengcc.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aty.sweek.top

[L03] 设置自定义请求头
来源：http://smt.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ixo.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jnc.316326.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gzs.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bmo.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zph.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dru.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yne.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hvi.fehbvm.com

[L04] 设置超时
来源：http://uxc.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://dsc.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lkz.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://enq.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fxv.hammf.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wge.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sle.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jyh.bbcook.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ppv.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://rpw.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qzz.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fgx.fzhhl.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nwn.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vgt.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://olc.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cld.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kgu.yj202588.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jaw.wangdashe.top

[L06] 解析响应为 JSON
来源：http://zth.yj202588.top

Py:   resp.json()
来源：http://pgq.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://xhu.hongshengwenyu.top

JS:   await resp.json()
来源：http://gof.dashuyun.cn

TS:   await resp.json()
来源：http://ape.fehbvm.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hde.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qpo.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://qja.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rru.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://huh.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cnj.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xjw.sjlbkw.cn

JS:   resp.ok;  resp.status
来源：http://mnb.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://ljc.yongpay.top

Java: resp.statusCode()
来源：http://uxo.fktsv.cn

Go:   resp.StatusCode
来源：http://egt.9152youxi.cn

Ruby: resp.code.to_i
来源：http://vku.shanyushiyangtech.top

C#:   (int)resp.StatusCode
来源：http://sru.yangfankeji.com

[L08] 并发请求多个地址
来源：http://bzx.redwolf501.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gup.shuidangran.top

PHP:  curl_multi_init() 系列
来源：http://khx.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ixw.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ngc.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kzn.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kxw.cqqwz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ryx.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qon.sysykeji.top

================================================================================
来源：http://elr.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://ipm.fehbvm.com

================================================================================
来源：http://otk.hnqzz.top

[M01] 读取命令行参数
来源：http://mkt.ybcxt.top

Py:   sys.argv[1:]
来源：http://uqo.yj20258888.top

PHP:  $argv;  $argc;
来源：http://usr.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://qee.andypj.xyz

TS:   process.argv.slice(2)
来源：http://nzu.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://max.tianlin.xyz

Go:   os.Args[1:]
来源：http://dkw.hongshengwenyu.top

Ruby: ARGV
来源：http://ztm.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://eod.jlsjyb.cn

[M02] 读取环境变量
来源：http://hgx.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://kod.hammf.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://knw.ydjk.org.cn

JS:   process.env.HOME
来源：http://vlc.iojbl.cn

TS:   process.env.HOME
来源：http://zru.hammf.cn

Java: System.getenv("HOME")
来源：http://xcl.c1oappe.top


<!-- 参考信息 -->