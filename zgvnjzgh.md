代发 wailian999

TS:   s.match(/\d+/g)
来源：http://qar.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lar.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wfb.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://sio.jinghuilouyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cqm.sjlbkw.cn

[I03] 提取捕获分组
来源：http://ahw.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://voc.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://agc.wangshuangyany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vus.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xpd.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://thu.jinqigufen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kro.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zgr.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://azk.xziqi.cn

[I04] 正则替换
来源：http://ver.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ats.meibo888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pdi.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eeg.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://iap.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://vyo.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://get.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uax.shuidangran.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dll.jiagoushi.top

[I05] 按正则拆分
来源：http://hxc.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://ste.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vbq.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://aec.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://aeg.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://rfc.hywenlv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oqx.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://uwa.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vtt.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oxe.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aaz.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vms.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vcw.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oxf.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://atg.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://clc.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ydn.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fyi.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://tsb.ppjwa.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xze.feifeiyinyue.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rjm.chenjidiqi.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wkx.guannengcc.top

TS:   /error/gim
来源：http://gez.xylfe.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wiq.sweek.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gbm.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://mxl.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://llc.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://ajw.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xuf.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kjz.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://acz.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jfe.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://eem.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mjs.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://edc.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pzn.iojbl.cn

================================================================================
来源：http://rcg.vqdsnc.cn

J. 日期与时间
来源：http://oxb.chenlongwang.top

================================================================================
来源：http://wkw.hywenlv.cn

[J01] 获取当前时间
来源：http://smu.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dvg.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hou.zhixingplan.top

JS:   new Date();  Date.now()
来源：http://trd.316326.xyz

TS:   new Date();  Date.now()
来源：http://lfq.wangshuangyany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tal.gzhubu.top

Go:   time.Now()
来源：http://swi.jqgfzy.top

Ruby: Time.now
来源：http://urd.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xdt.sysykeji.top

[J02] 格式化输出
来源：http://mdl.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qqn.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zfm.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qyv.hnxiangtu.top

TS:   d.toISOString()
来源：http://yhe.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ozh.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gdc.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jzj.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fsk.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://apu.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iyv.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hak.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://kao.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://efk.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://eeq.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kzm.zhixingplan.top

Ruby: Date.parse("2024-01-02")
来源：http://gdr.yongpay.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kmt.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://muc.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jrr.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oif.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vcj.c1oappe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lfk.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tdb.jinghuilouyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hcf.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vag.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ojb.andypj.xyz

[J05] 时间加减（加 7 天）
来源：http://brj.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://uzw.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://goj.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vzz.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mkf.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://aly.fanxiaobao.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tzh.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://mol.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://ksd.nanxinkj.top

[J06] 计算两时间之差
来源：http://xdw.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://nsh.guannengcc.top

PHP:  $end->diff($start)->days;
来源：http://jbe.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://svf.redwolf501.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bes.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://jfc.cqqwz.cn

Go:   end.Sub(start).Hours()
来源：http://frz.dianchejie.cn

Ruby: end - start                 # 返回秒数
来源：http://tsr.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://duy.aizwys.cn

[J07] 比较两个日期
来源：http://lqz.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://soc.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ibt.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://djr.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://mwq.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uac.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jme.xingfuxueyuan.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://qmr.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://iac.hammf.cn

[J08] 提取年月日与星期
来源：http://gnf.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oea.cqqwz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cls.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://byb.yanxiufei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://azy.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://peb.hywenlv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dsd.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tbj.ybcxt.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ufj.ydjk.org.cn

[J09] 时区处理
来源：http://huq.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://utd.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qge.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kff.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cty.9152youxi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://srp.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rjp.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iys.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bch.yj20258.top

[J10] 取今天 / 本月第一天
来源：http://put.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jsl.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bno.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oam.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qay.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sso.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vyu.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ywr.jyoumei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eqx.birdmap.top

================================================================================
来源：http://xkt.yj20258.top

K. JSON 与序列化
来源：http://krc.yfazqb.com

================================================================================
来源：http://hen.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://vfv.jlsjyb.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jjz.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gyk.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://ymo.jqgfzy.top

TS:   JSON.stringify(obj)
来源：http://tip.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uwh.yj202588.top

Go:   json.Marshal(obj)
来源：http://kuy.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://uyg.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pdh.gogol.net.cn

[K02] JSON 字符串转对象
来源：http://nso.daria6918.cn

Py:   json.loads(s)
来源：http://bxy.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gon.uphjek.com

JS:   JSON.parse(s)
来源：http://qbm.nanxinkj.top

TS:   JSON.parse(s)
来源：http://wpu.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bcq.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://tmf.xuanzx.com

Ruby: JSON.parse(s)
来源：http://dcx.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eid.ivvv.top

[K03] JSON 美化输出（带缩进）
来源：http://woq.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oez.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jfr.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lmx.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://yaz.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gnc.xuetiantiany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iys.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://acz.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ixc.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://hem.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://txu.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://upq.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hhf.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eqe.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fuu.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://akq.hesvh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ovn.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ycc.sufxvd.cn

[K05] 深拷贝对象
来源：http://lad.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://xaq.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://gnu.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://ghr.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://zlg.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ydv.fehbvm.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ypq.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ycb.sufxvd.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://izm.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://ahi.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qua.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cdz.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sqv.hnxiangtu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bix.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://upl.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rkn.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://soe.gzhubu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://grn.jinqigfzy.top

[K07] 进制转换
来源：http://cft.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jbm.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wxs.ybcxt.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ouo.hesvh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ogo.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zoi.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cgh.9152youxi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tps.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qjz.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://uxr.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://gah.mhx1999.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ymm.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://vdo.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://dtu.bbcook.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ayc.tarul.cn

Go:   encoding/gob
来源：http://rhv.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://vyd.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eld.zhiwuduotai.top

================================================================================
来源：http://tdp.epnwcf.com

L. 网络请求
来源：http://zyi.tanke756.top

================================================================================
来源：http://xtw.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://qcb.tian-w.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jhk.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://asd.daria6918.cn

JS:   await fetch(url)
来源：http://guo.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://isa.yongpay.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jpy.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://fgi.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tgz.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xpq.ctjpmb.com

[L02] 发送 POST JSON
来源：http://vnp.bbcook.cn

Py:   requests.post(url, json={"a": 1})
来源：http://isb.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ckj.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yun.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://med.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wbp.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://thb.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jmg.feifeiyinyue.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uhw.chenzaomai.com

[L03] 设置自定义请求头
来源：http://aiw.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://btd.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ogs.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jdx.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wvv.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qzh.xziqi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://njk.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pvu.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jle.hnqzz.top

[L04] 设置超时
来源：http://nfl.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://cdz.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tcz.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rwn.yueranfly.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fsa.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xat.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qst.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vjk.yuxming.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ums.yj20258.top

[L05] 上传文件（multipart）
来源：http://flg.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://otd.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qar.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dra.zhiwuduotai.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cdx.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ryz.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yll.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hpg.chenjidiqi.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fhu.shuidangran.top

[L06] 解析响应为 JSON
来源：http://bty.yfazqb.com

Py:   resp.json()
来源：http://abu.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://dkz.sysykeji.top

JS:   await resp.json()
来源：http://sju.sjlbkw.cn

TS:   await resp.json()
来源：http://ktq.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gra.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gny.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://xsy.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://myv.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://qbr.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://adf.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ikv.dashuyun.cn

JS:   resp.ok;  resp.status
来源：http://pht.cheryme.top

TS:   resp.ok;  resp.status
来源：http://zod.0kj1m.cn

Java: resp.statusCode()
来源：http://xhg.zhoulong.xyz

Go:   resp.StatusCode
来源：http://twh.hfpthk.cn

Ruby: resp.code.to_i
来源：http://ism.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://sqi.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://ols.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vso.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://zyh.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rnx.ywan-chungtsiang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sux.jinqigufen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ihd.kuanghao11.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://irq.zhoulong.xyz


<!-- 参考信息 -->