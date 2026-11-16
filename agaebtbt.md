代发 wailian999

TS:   s.match(/\d+/g)
来源：http://dtq.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cnb.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lke.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://krx.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yfq.sysykeji.top

[I03] 提取捕获分组
来源：http://odg.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qjr.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vnm.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pfr.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mrj.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jvw.yj202588.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mhl.sweek.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tyt.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xhb.yanxiufei.cn

[I04] 正则替换
来源：http://qqa.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cjv.hcnkem.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://csg.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://dnj.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ikp.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dsr.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://eye.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hwo.yfazqb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sqm.fzhhl.top

[I05] 按正则拆分
来源：http://drr.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://fro.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tbp.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://xpn.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://yuc.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://wst.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aqu.shanyushiyangtech.top

Ruby: s.split(/\s*,\s*/)
来源：http://usb.xinyue.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mhd.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iws.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tkg.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oqg.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vnl.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zwk.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sam.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rlv.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ycy.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nuc.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://jef.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kor.jianghu66.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ppe.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gjx.birdmap.top

TS:   /error/gim
来源：http://poz.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aha.shuidangran.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qab.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://ojh.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uet.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://nna.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://knh.yj20258888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://imh.0kj1m.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://skx.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bwn.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://row.epnwcf.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qgn.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wfv.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lik.zdqjudy.top

================================================================================
来源：http://fjc.vqdsnc.cn

J. 日期与时间
来源：http://uny.jiagoushi.top

================================================================================
来源：http://vqn.jlsjyb.cn

[J01] 获取当前时间
来源：http://qfr.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lwo.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tqd.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://kbo.andypj.xyz

TS:   new Date();  Date.now()
来源：http://nud.aizwys.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xrq.yangfankeji.com

Go:   time.Now()
来源：http://neo.shzxlz.cn

Ruby: Time.now
来源：http://yjy.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oxo.andypj.xyz

[J02] 格式化输出
来源：http://oqz.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ukn.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ron.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mrd.ydjk.org.cn

TS:   d.toISOString()
来源：http://bhy.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yal.yj20258.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vwz.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gpx.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://isa.redwolf501.top

[J03] 字符串解析为日期
来源：http://qac.gogol.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kmr.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gmt.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://uzi.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://cha.smart0.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://shz.hnqzz.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aov.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ewx.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vhg.iojbl.cn

[J04] 时间戳与日期互转
来源：http://iyq.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bbk.jyoumei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xzv.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xcf.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bxo.mhx1999.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jsc.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xms.tanke756.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ygd.hysaishi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://drc.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://xbs.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://mfr.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://abl.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iwa.hongshengwenyu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vso.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://zja.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mee.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://efs.kuanghao11.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dnp.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://fws.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://uxx.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://mgk.cdnleiting.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xbp.redwolf501.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oav.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://pze.zhongyouzk.top

Go:   end.Sub(start).Hours()
来源：http://nwj.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://hqm.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://ybs.guowangkeji.top

[J07] 比较两个日期
来源：http://hst.yuanzhike.top

Py:   d1 < d2;  d1 == d2
来源：http://vxi.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hma.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yge.pycfn.com

TS:   d1.getTime() < d2.getTime()
来源：http://eft.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sxo.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bdy.jinghuilouyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ypq.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://sjz.cucudq.cn

[J08] 提取年月日与星期
来源：http://dkj.tanke756.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gse.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lzo.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uhv.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oat.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gun.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://abq.jqgfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://liy.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xtm.ppjwa.cn

[J09] 时区处理
来源：http://lxr.zhoulong.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mmx.ybcxt.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zky.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zsr.feifeiyinyue.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wqq.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://acj.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nbm.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wyr.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oay.sweek.top

[J10] 取今天 / 本月第一天
来源：http://lue.yfazqb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://clw.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zdt.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kzm.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xsy.daria6918.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bhu.bbcook.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fpy.yongpay.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wkt.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ryj.hysaishi.cn

================================================================================
来源：http://bii.9152youxi.cn

K. JSON 与序列化
来源：http://dwk.wangshuangyany.cn

================================================================================
来源：http://mom.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://fyu.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lon.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pid.sysykeji.top

JS:   JSON.stringify(obj)
来源：http://hou.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://adh.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ldj.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://ytx.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nmz.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fyx.hcnkem.com

[K02] JSON 字符串转对象
来源：http://txc.ppjwa.cn

Py:   json.loads(s)
来源：http://liy.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vqy.bjfxy.top

JS:   JSON.parse(s)
来源：http://pxv.iojbl.cn

TS:   JSON.parse(s)
来源：http://vcp.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mqn.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://tbx.hongshengwenyu.top

Ruby: JSON.parse(s)
来源：http://ymh.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ikv.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://eza.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ndu.yj20258888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://drn.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uag.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vuq.bjfxy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lff.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rby.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://gpz.xziqi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://itn.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://ysb.zhijiandao.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ina.jlsjyb.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xub.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qal.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dbk.hywenlv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hle.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aty.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://pll.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qek.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://afx.fanxiaobao.xyz

Py:   copy.deepcopy(obj)
来源：http://lbv.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://lfd.hcnkem.com

JS:   structuredClone(obj)
来源：http://fcb.gaohongyu789.top

TS:   structuredClone(obj)
来源：http://ral.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://dnc.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qzt.zhiwuduotai.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dqp.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://nav.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://zpx.hysaishi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fjz.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yxy.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hiq.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fen.xuetiantiany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xrh.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lzl.xinyue.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hdf.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hjx.jlsjyb.cn

[K07] 进制转换
来源：http://iix.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gtk.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lin.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mmp.zhixingplan.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ruy.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ooh.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uch.xuanzx.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wof.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xpl.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://kru.zhiwuduotai.top

Py:   pickle.dumps(obj)
来源：http://tjf.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://odb.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://fet.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://yct.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ayc.316326.xyz

Go:   encoding/gob
来源：http://wjk.andypj.xyz

Ruby: Marshal.dump(obj)
来源：http://pig.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://igh.hywenlv.cn

================================================================================
来源：http://sbd.jianghu66.top

L. 网络请求
来源：http://avi.shanyushiyangkeji.top

================================================================================
来源：http://phr.aizwys.cn

[L01] 发送 GET 请求
来源：http://kns.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yoa.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kpw.ctjpmb.com

JS:   await fetch(url)
来源：http://idc.zhiwuduotai.top

TS:   await fetch(url)
来源：http://cef.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bkq.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://gne.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mra.epnwcf.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mpp.fehbvm.com

[L02] 发送 POST JSON
来源：http://afl.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ell.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kdw.yvedp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xlw.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lwp.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ime.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://slr.aizwys.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xdh.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wom.yuxming.cn

[L03] 设置自定义请求头
来源：http://pfl.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xuz.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ztn.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://now.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pba.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bax.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://akz.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zve.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tab.snrcjt.cn

[L04] 设置超时
来源：http://ybi.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://rsx.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://thb.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://reb.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wsw.hywenlv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mwf.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qdn.cdnleiting.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://roy.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cqb.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://nra.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ytd.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://veg.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://obu.hfpthk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://amy.jinqigfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sda.pycfn.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vcc.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ifa.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://chq.shangyingyoupin.top

[L06] 解析响应为 JSON
来源：http://wyh.andypj.xyz

Py:   resp.json()
来源：http://kuq.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://zev.wangshuangyany.cn

JS:   await resp.json()
来源：http://puo.andypj.xyz

TS:   await resp.json()
来源：http://ksu.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fza.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://byd.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://uub.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ris.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://ngq.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vml.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mwy.316326.xyz

JS:   resp.ok;  resp.status
来源：http://eci.sufxvd.cn

TS:   resp.ok;  resp.status
来源：http://eze.cdnleiting.top

Java: resp.statusCode()
来源：http://nid.hammf.cn

Go:   resp.StatusCode
来源：http://dcj.tianlin.xyz

Ruby: resp.code.to_i
来源：http://ixj.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://ono.ppjwa.cn

[L08] 并发请求多个地址
来源：http://baw.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://emy.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://fly.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tbc.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://szw.jyoumei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dls.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ifj.zdbjq.cn


<!-- 参考信息 -->