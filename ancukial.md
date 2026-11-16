代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kbg.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pqu.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qao.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uze.52xcode.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://thw.tianlin.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://noi.bjfxy.top

[I04] 正则替换
来源：http://jvu.ehwqpu.com

Py:   re.sub(r"\d+", "#", s)
来源：http://wid.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rus.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://xmd.jinqigfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://yvm.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://gdh.zhengqikj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://syd.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ggu.xylfe.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://row.aibaodan.cn

[I05] 按正则拆分
来源：http://kbq.fehbvm.com

Py:   re.split(r"\s*,\s*", s)
来源：http://tbd.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ofu.yvedp.cn

JS:   s.split(/\s*,\s*/)
来源：http://qrh.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://nfj.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://nff.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ftt.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lxl.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xrk.sweek.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dhr.hfpthk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vhi.mhx1999.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ztn.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mvi.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sux.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qrq.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qsf.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gar.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tgz.cheryme.top

[I07] 忽略大小写与多行模式
来源：http://pmy.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wqh.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gvv.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dwh.bbcook.cn

TS:   /error/gim
来源：http://kuo.fktsv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yeb.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gzo.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://tmo.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pxs.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://hpp.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://brn.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uqb.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gjs.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ofu.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fjk.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://klt.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://giv.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tjf.jyoumei.cn

================================================================================
来源：http://wrd.dashuyun.cn

J. 日期与时间
来源：http://kpt.cqqwz.cn

================================================================================
来源：http://lry.hongshengwenyu.top

[J01] 获取当前时间
来源：http://jdw.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ksy.zhixingplan.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wnq.wangdashe.top

JS:   new Date();  Date.now()
来源：http://nbf.hfpthk.cn

TS:   new Date();  Date.now()
来源：http://jlg.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xqt.gaohongyu789.top

Go:   time.Now()
来源：http://dio.iojbl.cn

Ruby: Time.now
来源：http://swe.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qcu.zhiwuduotai.top

[J02] 格式化输出
来源：http://jmm.zdqjudy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://reg.svipenyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xrc.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://boh.hnqzz.top

TS:   d.toISOString()
来源：http://pgg.redwolf501.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ucs.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lze.fengsongda.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ppo.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gyc.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://bjk.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rij.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://itu.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://ylg.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://usu.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://tmf.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://obo.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://xgb.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kta.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://lgr.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kit.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ivo.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://htd.shanyushiyangtech.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ijd.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ajl.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hzp.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://khj.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yel.iojbl.cn

[J05] 时间加减（加 7 天）
来源：http://rpk.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://osp.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://kcw.zdqjudy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cle.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cls.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://sci.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uqj.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://ihh.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://xui.hfpthk.cn

[J06] 计算两时间之差
来源：http://pfu.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://edt.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://xme.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wov.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://llv.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bml.vqdsnc.cn

Go:   end.Sub(start).Hours()
来源：http://ylu.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://ahw.aibaodan.cn

C#:   (end - start).TotalSeconds
来源：http://ibi.zdqjudy.top

[J07] 比较两个日期
来源：http://yjc.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://uut.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pgx.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://myu.zhoulong.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://tke.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gde.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ykq.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://qip.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://wzd.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://ril.jinqigfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nje.hammf.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gft.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pcq.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fwy.sweek.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dex.52xcode.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rfn.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sos.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://urk.ehwqpu.com

[J09] 时区处理
来源：http://lam.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://she.zhixingplan.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qnp.fehbvm.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yap.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eaf.jyoumei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jtw.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tkv.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kdi.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fkk.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://rld.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://prz.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jwp.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rbv.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zcb.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ekr.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://icn.meibo888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xdn.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oud.jlsjyb.cn

================================================================================
来源：http://yws.hesvh.cn

K. JSON 与序列化
来源：http://trh.cqqwz.cn

================================================================================
来源：http://iyp.hnxiangtu.top

[K01] 对象转 JSON 字符串
来源：http://wge.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gvx.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ppi.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://bin.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://moy.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://stg.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://ssy.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ede.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jsd.yanxiufei.cn

[K02] JSON 字符串转对象
来源：http://vxi.pycfn.com

Py:   json.loads(s)
来源：http://etu.shangyingyoupin.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mxl.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://bsj.sysykeji.top

TS:   JSON.parse(s)
来源：http://jjn.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aje.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://wyq.bbcook.cn

Ruby: JSON.parse(s)
来源：http://eds.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://swy.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://ylr.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vtg.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://htt.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uxp.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qje.fengsongda.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mdw.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://alp.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://kzg.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uma.fehbvm.com

[K04] 读取 JSON 文件
来源：http://man.jiagoushi.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bwx.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zjm.jinqigufen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tdc.yueranfly.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://acv.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bzy.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bnp.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jdj.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pil.jyoumei.cn

[K05] 深拷贝对象
来源：http://jzx.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://ira.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://gvr.cheryme.top

JS:   structuredClone(obj)
来源：http://yro.redwolf501.top

TS:   structuredClone(obj)
来源：http://rbn.havefunace.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fcz.jinghuilouyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yex.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xof.tarul.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uhh.daxiang520.top

[K06] 解析 URL 查询串
来源：http://qie.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pev.fengsongda.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xoc.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rcl.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rpo.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tqo.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://voq.wangshuangyany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jik.bbcook.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fes.shangyingyoupin.top

[K07] 进制转换
来源：http://gzo.quarkkingdee.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bcc.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pec.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eiq.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://psj.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pqp.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qqo.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uku.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fqm.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://zpv.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://ykj.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://czz.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://vry.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://xrp.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xcf.yj202588.top

Go:   encoding/gob
来源：http://nfg.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://fdx.fengsongda.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://soc.wangdashe.top

================================================================================
来源：http://abn.guannengcc.top

L. 网络请求
来源：http://vji.smart0.xyz

================================================================================
来源：http://nro.jianghu66.top

[L01] 发送 GET 请求
来源：http://non.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://idu.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pmi.jqgfzy.top

JS:   await fetch(url)
来源：http://bsm.pengpengdd.cyou

TS:   await fetch(url)
来源：http://zfh.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bdu.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://rty.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ztz.dashuyun.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hnx.gzhubu.top

[L02] 发送 POST JSON
来源：http://oem.fktsv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qsm.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rcl.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dhz.chenjidiqi.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hne.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ifl.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iee.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tas.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://noh.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://qzr.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mmj.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wgc.tian-w.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dms.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wpw.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vvp.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vwj.sjlbkw.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uth.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ydc.zhiwuduotai.top

[L04] 设置超时
来源：http://apn.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://iku.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sqo.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ovb.gzhubu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wtj.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rao.xinyue.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qky.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://glm.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mrk.havefunace.top

[L05] 上传文件（multipart）
来源：http://hak.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pfs.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dxp.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fmb.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dhx.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ves.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mcf.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wuo.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qjh.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://ekx.fanxiaobao.xyz

Py:   resp.json()
来源：http://nhn.yfazqb.com

PHP:  json_decode($body, true);
来源：http://pkw.sweek.top

JS:   await resp.json()
来源：http://dym.vqdsnc.cn

TS:   await resp.json()
来源：http://jkq.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://etd.xingfuxueyuan.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wjn.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://zii.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qem.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://gje.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zsd.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://acl.smart0.xyz

JS:   resp.ok;  resp.status
来源：http://tzg.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://sgx.pengpengdd.cyou

Java: resp.statusCode()
来源：http://zxt.hnqzz.top

Go:   resp.StatusCode
来源：http://mfn.fktsv.cn

Ruby: resp.code.to_i
来源：http://nif.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://scd.tanke756.top

[L08] 并发请求多个地址
来源：http://alg.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wny.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://fgd.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://llp.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gnn.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hta.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tca.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wdr.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xyb.hysaishi.cn

================================================================================
来源：http://vob.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://uaz.nwbrower.top

================================================================================
来源：http://hnd.shuidangran.top

[M01] 读取命令行参数
来源：http://epw.xuanzx.com

Py:   sys.argv[1:]
来源：http://zqx.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://ppj.c1oappe.top


<!-- 参考信息 -->