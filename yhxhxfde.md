代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kqh.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ubn.ybcxt.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bef.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://orn.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cke.yangfankeji.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wng.sysykeji.top

[I04] 正则替换
来源：http://zwu.cqqwz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://emu.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hjv.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://fgi.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bcc.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://trs.pycfn.com

Go:   re.ReplaceAllString(s, "#")
来源：http://syn.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://erh.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ece.fktsv.cn

[I05] 按正则拆分
来源：http://kaf.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://wut.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pre.yj202588.top

JS:   s.split(/\s*,\s*/)
来源：http://yng.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://klu.ehwqpu.com

Java: s.split("\\s*,\\s*")
来源：http://ibs.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tzu.tanke756.top

Ruby: s.split(/\s*,\s*/)
来源：http://rno.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kki.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iah.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://amb.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uij.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wyz.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rut.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ofp.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://abw.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mrq.jqgufenzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kxm.cqqwz.cn

[I07] 忽略大小写与多行模式
来源：http://rgv.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xje.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jwv.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cck.tanke756.top

TS:   /error/gim
来源：http://dsf.ctjpmb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rfa.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gse.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://ukt.zhoulong.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wfm.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://wiq.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hre.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hxk.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ygt.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aml.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://znh.pengpengdd.cyou

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://woo.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tns.pycfn.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zvq.cashguo.top

================================================================================
来源：http://uur.hnxiangtu.top

J. 日期与时间
来源：http://rkr.aizwys.cn

================================================================================
来源：http://mlo.sjlbkw.cn

[J01] 获取当前时间
来源：http://gsi.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://xso.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cxd.yj202588.top

JS:   new Date();  Date.now()
来源：http://yol.fengsongda.top

TS:   new Date();  Date.now()
来源：http://chf.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oyj.meibo888.top

Go:   time.Now()
来源：http://qze.daria6918.cn

Ruby: Time.now
来源：http://rts.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tml.cheryme.top

[J02] 格式化输出
来源：http://fib.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sxd.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yrq.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kap.vehdjk.com

TS:   d.toISOString()
来源：http://ane.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mnk.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qch.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bki.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://awi.jinqigufen.top

[J03] 字符串解析为日期
来源：http://drg.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dkd.guannengcc.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ohd.9152youxi.cn

JS:   new Date("2024-01-02")
来源：http://iol.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://odb.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://bpn.jinyuanbaomall.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yin.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://rdr.yuxming.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://toh.xinyue.icu

[J04] 时间戳与日期互转
来源：http://gvz.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://geo.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lbf.zhiwuduotai.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wax.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kyw.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blz.hywenlv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ncy.andypj.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://som.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rhe.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://txy.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://iie.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yye.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ugc.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qsp.fengsongda.top

Java: LocalDate.now().plusDays(7)
来源：http://ahc.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ogw.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://tbq.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oip.jqgufenzy.top

[J06] 计算两时间之差
来源：http://ery.gzhubu.top

Py:   (end - start).total_seconds()
来源：http://ebs.ctjpmb.com

PHP:  $end->diff($start)->days;
来源：http://aoe.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aix.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://omb.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://xha.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://kpy.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://ivz.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://emu.sjlbkw.cn

[J07] 比较两个日期
来源：http://twy.jiagoushi.top

Py:   d1 < d2;  d1 == d2
来源：http://fan.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wkf.hfpthk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tls.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://igj.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zda.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ent.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://xet.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://oot.yuxming.cn

[J08] 提取年月日与星期
来源：http://qbl.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mqb.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cdy.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lhn.yanxiufei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dwv.zdbjq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dhf.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pim.hnqzz.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wle.svipenyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://auo.sufxvd.cn

[J09] 时区处理
来源：http://zkc.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iwe.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://klq.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://opu.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jbz.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xwk.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://deh.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qvh.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jbt.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://rvw.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rmz.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fua.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iln.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wof.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iuo.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iqq.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dyy.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://heg.guowangkeji.top

================================================================================
来源：http://zvm.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://mmt.ydjk.org.cn

================================================================================
来源：http://cjd.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://oxk.yj20258.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yje.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iha.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://htq.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://czw.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kzc.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://frg.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oql.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://epe.ivvv.top

[K02] JSON 字符串转对象
来源：http://nux.ctjpmb.com

Py:   json.loads(s)
来源：http://tqm.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fce.fengsongda.top

JS:   JSON.parse(s)
来源：http://cja.zhaomingkeji.xyz

TS:   JSON.parse(s)
来源：http://cny.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vuw.yuxming.cn

Go:   json.Unmarshal(data, &v)
来源：http://rgr.hcnkem.com

Ruby: JSON.parse(s)
来源：http://uhc.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ogd.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://dpe.yangfankeji.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://arx.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hkc.hammf.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tcv.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://awt.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ckq.316326.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ieo.meibo888.top

Ruby: JSON.pretty_generate(obj)
来源：http://vsc.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yyd.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://tbe.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vqk.zhiwuduotai.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tbd.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://crd.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zsb.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nrn.yonumen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://psq.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vkw.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gmx.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://vdf.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://seb.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://abr.wangdashe.top

JS:   structuredClone(obj)
来源：http://uul.redwolf501.top

TS:   structuredClone(obj)
来源：http://xet.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ymw.jinyuanbaomall.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://htr.hesvh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ixx.shanyushiyangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sjm.hesvh.cn

[K06] 解析 URL 查询串
来源：http://wwd.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://czq.jinghuilouyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://shh.yj20258.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rmv.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tux.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bvx.quarkkingdee.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://arl.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oyr.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qal.quarkkingdee.top

[K07] 进制转换
来源：http://qgz.havefunace.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eiw.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hsv.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tfu.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vcx.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jsq.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lvc.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fkf.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cqu.jinyuanbaomall.cn

[K08] 二进制序列化（非 JSON）
来源：http://xxa.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://anv.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dfa.cdnleiting.top

JS:   v8.serialize(obj)        // Node
来源：http://zrh.daxiang520.top

TS:   v8.serialize(obj)        // Node
来源：http://nyr.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://elm.andypj.xyz

Go:   encoding/gob
来源：http://zlw.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://phi.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://msr.hywenlv.cn

================================================================================
来源：http://ijb.ybcxt.top

L. 网络请求
来源：http://kue.wangdashe.top

================================================================================
来源：http://qaq.feifeiyinyue.top

[L01] 发送 GET 请求
来源：http://yzp.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rqh.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bhc.jinqigufen.top

JS:   await fetch(url)
来源：http://nrf.andypj.xyz

TS:   await fetch(url)
来源：http://aua.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jlg.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://zvs.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vbm.gaohongyu789.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cpr.316326.xyz

[L02] 发送 POST JSON
来源：http://tfn.fktsv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://awz.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bpd.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://edy.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://crr.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cqk.fengsongda.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qyl.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fqc.hysaishi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ysy.nanxinkj.top

[L03] 设置自定义请求头
来源：http://zek.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tfq.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jay.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ict.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xrt.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dje.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xde.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nfs.vqdsnc.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ktv.0kj1m.cn

[L04] 设置超时
来源：http://rvv.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://hpx.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://suv.wangdashe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tmr.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bps.zhaomingkeji.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pti.ybcxt.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fzt.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nke.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nxi.hammf.cn

[L05] 上传文件（multipart）
来源：http://akr.zycfv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zvc.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://khk.daria6918.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cfr.gogol.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dnd.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://frc.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lgl.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vog.aibaodan.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://roc.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://ztx.pycfn.com

Py:   resp.json()
来源：http://gxz.yvedp.cn

PHP:  json_decode($body, true);
来源：http://otp.iojbl.cn

JS:   await resp.json()
来源：http://vri.pengpengdd.cyou

TS:   await resp.json()
来源：http://oup.sjlbkw.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://for.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://joh.xylfe.cn

Ruby: JSON.parse(resp.body)
来源：http://ecc.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bee.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://qzy.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hif.iojbl.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ktp.sjlbkw.cn

JS:   resp.ok;  resp.status
来源：http://meq.tarul.cn

TS:   resp.ok;  resp.status
来源：http://pdy.xylfe.cn

Java: resp.statusCode()
来源：http://mkd.yangfankeji.com

Go:   resp.StatusCode
来源：http://wnu.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://ibb.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://eqz.yangfankeji.com

[L08] 并发请求多个地址
来源：http://lvy.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wge.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://cbh.jinghuilouyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oqd.sysykeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://klf.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tnc.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gfg.jlsjyb.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://irh.yanxiufei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fww.guowangkeji.top

================================================================================
来源：http://rpz.epnwcf.com

M. 命令行 / 进程 / 环境
来源：http://yop.bbcook.cn

================================================================================
来源：http://btr.wangdashe.top

[M01] 读取命令行参数
来源：http://uwt.cheryme.top

Py:   sys.argv[1:]
来源：http://rbc.guannengcc.top

PHP:  $argv;  $argc;
来源：http://qoa.jyoumei.cn


<!-- 参考信息 -->