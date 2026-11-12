代发 wailian999

TS:   s.match(/\d+/g)
来源：http://cwk.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bsz.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fvo.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://mru.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rmh.hcnkem.com

[I03] 提取捕获分组
来源：http://rmt.tarul.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pqf.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fqe.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sda.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qek.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vbi.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fyd.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cys.andypj.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lwp.hongshengwenyu.top

[I04] 正则替换
来源：http://qzk.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dpx.bjfxy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mej.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://dot.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://vsl.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://duh.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rui.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nut.hywenlv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xvs.sjlbkw.cn

[I05] 按正则拆分
来源：http://mrz.ppjwa.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bdw.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://szd.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://vpk.nanxuanxn.top

TS:   s.split(/\s*,\s*/)
来源：http://emq.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://tbu.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hey.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://hdv.cqqwz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bcb.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iet.9152youxi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://niu.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dcg.gaohongyu789.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fsw.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://khk.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uom.ybcxt.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xaj.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tyv.fehbvm.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yqm.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://zvk.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://csc.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gys.dashuyun.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://doq.dashuyun.cn

TS:   /error/gim
来源：http://ckd.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pxk.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ajx.ivvv.top

Ruby: s.scan(/error/i)
来源：http://lxh.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lku.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://ohw.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cbn.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ytf.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sbb.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bnh.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ihz.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eco.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ybn.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qkt.hnxiangtu.top

================================================================================
来源：http://mcb.aibaodan.cn

J. 日期与时间
来源：http://mko.jqgufenzy.top

================================================================================
来源：http://pos.xuetiantiany.cn

[J01] 获取当前时间
来源：http://rrb.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://oxj.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gob.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://hzc.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://kka.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://luv.jqgfzy.top

Go:   time.Now()
来源：http://rly.bjfxy.top

Ruby: Time.now
来源：http://mjs.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zna.zhengqikj.top

[J02] 格式化输出
来源：http://cmf.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wro.cqqwz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ovb.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iqg.zhiwuduotai.top

TS:   d.toISOString()
来源：http://kzg.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yzv.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ndl.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qyz.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://owh.yangfankeji.com

[J03] 字符串解析为日期
来源：http://jwc.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ifz.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bvk.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://ufs.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://yjn.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bem.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cmp.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://qms.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mjc.pycfn.com

[J04] 时间戳与日期互转
来源：http://qhy.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qei.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ugo.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uow.guowangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jll.zhoulong.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pds.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fjw.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eeq.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://glb.yangfankeji.com

[J05] 时间加减（加 7 天）
来源：http://kdr.tarul.cn

Py:   now + timedelta(days=7)
来源：http://gpr.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://mhb.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hhu.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hhj.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://cyb.shanyushiyangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ktk.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://zwe.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://kyh.snrcjt.cn

[J06] 计算两时间之差
来源：http://aeu.guowangkeji.top

Py:   (end - start).total_seconds()
来源：http://skf.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://yox.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uqg.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ife.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://vtv.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://stb.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://onf.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://llk.jinqigfzy.top

[J07] 比较两个日期
来源：http://ola.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://oxc.shangyingyoupin.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hya.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hsk.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://dgv.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hbt.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://whl.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://cvs.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://pot.svipenyu.cn

[J08] 提取年月日与星期
来源：http://fhi.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lpd.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fph.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sfb.wangshuangyany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qkz.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vda.tarul.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fqj.cqqwz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://udh.ydzc1.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kbj.tian-w.cn

[J09] 时区处理
来源：http://bay.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tqg.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lza.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mvi.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qeh.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vdi.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ozt.jianghu66.top

Ruby: Time.now.getlocal("+08:00")
来源：http://urr.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yuv.yuxming.cn

[J10] 取今天 / 本月第一天
来源：http://zbo.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vjj.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bcn.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uuc.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rvy.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yra.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qeg.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wzh.nanxuanxn.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pnp.0kj1m.cn

================================================================================
来源：http://wdg.cqqwz.cn

K. JSON 与序列化
来源：http://lta.jlsjyb.cn

================================================================================
来源：http://psv.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://sve.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://igi.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pwf.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://ort.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://mbg.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dhs.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://rcr.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://ceu.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lcp.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://svs.gotoacloud.top

Py:   json.loads(s)
来源：http://lna.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jll.xylfe.cn

JS:   JSON.parse(s)
来源：http://maa.dianchejie.cn

TS:   JSON.parse(s)
来源：http://noa.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ybg.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://zaq.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://oml.cheryme.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fmi.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ahm.tian-w.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bgg.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ftw.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qdh.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hnd.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ahh.dashuyun.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mgw.sjlbkw.cn

Ruby: JSON.pretty_generate(obj)
来源：http://psh.jianghu66.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fcf.meibo888.top

[K04] 读取 JSON 文件
来源：http://pdy.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cgw.xuanzx.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jki.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aeb.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xld.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yel.meibo888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zhc.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://qmn.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zup.cashguo.top

[K05] 深拷贝对象
来源：http://law.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://law.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://vyz.pycfn.com

JS:   structuredClone(obj)
来源：http://dyo.zdqjudy.top

TS:   structuredClone(obj)
来源：http://npi.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qwo.zhengqikj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://has.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kgw.zdbjq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vak.wangshuangyany.cn

[K06] 解析 URL 查询串
来源：http://rum.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fdk.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bud.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fpv.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sxy.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iuo.cheryme.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zgr.c1oappe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wrg.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://srg.fengsongda.top

[K07] 进制转换
来源：http://kqp.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kwi.tian-w.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://abc.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cet.bjfxy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qkk.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sop.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ktg.zycfv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://prj.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zod.sxryk.cn

[K08] 二进制序列化（非 JSON）
来源：http://lpk.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://bfv.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://pwo.dianchejie.cn

JS:   v8.serialize(obj)        // Node
来源：http://mln.bjfxy.top

TS:   v8.serialize(obj)        // Node
来源：http://vey.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://izc.smart0.xyz

Go:   encoding/gob
来源：http://eaz.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://jiz.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ulc.chenlongwang.top

================================================================================
来源：http://kup.hysaishi.cn

L. 网络请求
来源：http://auj.ydzc1.top

================================================================================
来源：http://wbb.hnqzz.top

[L01] 发送 GET 请求
来源：http://inw.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iip.hnqzz.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rqr.sufxvd.cn

JS:   await fetch(url)
来源：http://cge.jianghu66.top

TS:   await fetch(url)
来源：http://zjw.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nms.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://xok.jlsjyb.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jnz.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uip.yongpay.top

[L02] 发送 POST JSON
来源：http://tyh.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fys.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sac.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kxf.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yew.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://scd.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://izz.shzxlz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vgy.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xed.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://ska.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pkk.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://met.shanyushiyangtech.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uoo.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vtk.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dvh.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gab.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pbh.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kjh.52xcode.cn

[L04] 设置超时
来源：http://ifz.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://nbc.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://psk.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gkw.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uld.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vun.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sao.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://czu.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://chu.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://ros.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bdc.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oqg.fanxiaobao.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dup.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mvr.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mra.jqgfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yqf.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pqb.tarul.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xuf.tarul.cn

[L06] 解析响应为 JSON
来源：http://eat.jianghu66.top

Py:   resp.json()
来源：http://fby.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://gsu.dashuyun.cn

JS:   await resp.json()
来源：http://eee.ydjk.org.cn

TS:   await resp.json()
来源：http://sfe.gaohongyu789.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://efy.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mjb.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://tyl.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ipk.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://iaf.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xeh.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hdt.daxiang520.top

JS:   resp.ok;  resp.status
来源：http://hmg.c1oappe.top

TS:   resp.ok;  resp.status
来源：http://znh.hesvh.cn

Java: resp.statusCode()
来源：http://wvm.xinyue.icu

Go:   resp.StatusCode
来源：http://amz.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://ucf.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://ook.gzhubu.top

[L08] 并发请求多个地址
来源：http://txd.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://boz.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://bxd.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fze.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://egg.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qns.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xen.bjfxy.top


<!-- 参考信息 -->