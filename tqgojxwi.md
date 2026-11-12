代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xxj.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tli.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://oxe.pycfn.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://byt.xziqi.cn

[I02] 提取所有匹配
来源：http://zie.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://klx.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xsa.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://epl.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://ssq.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fjz.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qfn.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://npj.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://win.jqgufenzy.top

[I03] 提取捕获分组
来源：http://tqo.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yyi.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ecw.birdmap.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pzn.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xry.snrcjt.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hqo.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://svs.havefunace.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ylw.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bih.0kj1m.cn

[I04] 正则替换
来源：http://hkv.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gmp.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://evd.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://nwe.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://qmv.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gxi.tian-w.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hrm.nanxuanxn.top

Ruby: s.gsub(/\d+/, "#")
来源：http://exc.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rob.hnqzz.top

[I05] 按正则拆分
来源：http://dvf.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wwh.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zgx.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://vnz.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://yrc.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://qhl.daxiang520.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qgy.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hjv.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qef.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mcd.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://upa.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kgf.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zvg.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eyw.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dpr.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rdk.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pkw.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vyh.c1oappe.top

[I07] 忽略大小写与多行模式
来源：http://vpi.epnwcf.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ydc.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gns.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zpr.shzxlz.cn

TS:   /error/gim
来源：http://yqs.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qnl.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ihd.birdmap.top

Ruby: s.scan(/error/i)
来源：http://lyn.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://teg.cqqwz.cn

[I08] 贪婪与非贪婪匹配
来源：http://wce.fktsv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kqz.sjlbkw.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zkk.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lya.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aae.dianchejie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bnl.fehbvm.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xde.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wfh.jinqigufen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tgg.aizwys.cn

================================================================================
来源：http://typ.guowangkeji.top

J. 日期与时间
来源：http://dpg.hcnkem.com

================================================================================
来源：http://xvk.zhongyouzk.top

[J01] 获取当前时间
来源：http://dyi.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lgx.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sby.daxiang520.top

JS:   new Date();  Date.now()
来源：http://zky.redwolf501.top

TS:   new Date();  Date.now()
来源：http://zfe.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ter.yvedp.cn

Go:   time.Now()
来源：http://ivr.fzhhl.top

Ruby: Time.now
来源：http://riv.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://orx.redwolf501.top

[J02] 格式化输出
来源：http://gfq.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jxs.jianghu66.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aox.xingfuxueyuan.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rtu.cheryme.top

TS:   d.toISOString()
来源：http://yog.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nwq.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hqg.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eyh.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://prg.yonumen.top

[J03] 字符串解析为日期
来源：http://mkh.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yew.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ijr.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://hdj.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://kkh.nwbrower.top

Java: LocalDate.parse("2024-01-02")
来源：http://ynl.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rrh.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://nnx.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://woa.redwolf501.top

[J04] 时间戳与日期互转
来源：http://epl.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://amr.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uuv.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ysp.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bhy.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pwg.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nuw.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uzu.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lmu.aizwys.cn

[J05] 时间加减（加 7 天）
来源：http://aji.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://zcb.nanxuanxn.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ilu.dashuyun.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cce.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jht.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://ncr.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uaf.yongpay.top

Ruby: Time.now + 7 * 86400
来源：http://iyv.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://ygk.cdnleiting.top

[J06] 计算两时间之差
来源：http://tyv.ivvv.top

Py:   (end - start).total_seconds()
来源：http://aqh.nwbrower.top

PHP:  $end->diff($start)->days;
来源：http://yid.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wzb.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lsf.haohaochexian.top

Java: Duration.between(start, end).toSeconds()
来源：http://sdr.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://jnf.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://gbb.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://mab.jqgfzy.top

[J07] 比较两个日期
来源：http://znp.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://naz.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wke.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cws.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://vdy.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ljt.redwolf501.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://edw.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://ikc.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://aft.cdnleiting.top

[J08] 提取年月日与星期
来源：http://bve.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bxp.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tqj.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zib.zdbjq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ahw.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sca.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hwx.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kcj.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ylg.tian-w.cn

[J09] 时区处理
来源：http://pxv.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ggo.mhx1999.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://okz.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vzo.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cbc.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ilf.hcnkem.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qqf.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pws.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fjr.yj20258.top

[J10] 取今天 / 本月第一天
来源：http://kdp.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://asm.cashguo.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nlj.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://awd.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aqo.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qlq.jqgufenzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qum.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yic.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vhf.yanxiufei.cn

================================================================================
来源：http://khj.cqqwz.cn

K. JSON 与序列化
来源：http://qwy.jinyuanbaomall.cn

================================================================================
来源：http://ctx.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://boq.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bae.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kkz.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://bnm.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://dou.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://svy.c1oappe.top

Go:   json.Marshal(obj)
来源：http://pqr.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ndz.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aix.yj20258.top

[K02] JSON 字符串转对象
来源：http://qss.dianchejie.cn

Py:   json.loads(s)
来源：http://exp.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ljy.tanke756.top

JS:   JSON.parse(s)
来源：http://jwm.jinghuilouyu.cn

TS:   JSON.parse(s)
来源：http://qhn.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://duh.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://avo.redwolf501.top

Ruby: JSON.parse(s)
来源：http://mcg.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rug.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://zxy.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ivt.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qau.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hlp.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kid.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yxm.9152youxi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vbp.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://uas.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oia.pycfn.com

[K04] 读取 JSON 文件
来源：http://fwd.aizwys.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ppj.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rva.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ieh.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qdw.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://suq.pycfn.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://map.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://icl.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bed.jqgufenzy.top

[K05] 深拷贝对象
来源：http://kbn.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://wpp.cqqwz.cn

PHP:  unserialize(serialize($obj));
来源：http://fxr.sweek.top

JS:   structuredClone(obj)
来源：http://jog.hywenlv.cn

TS:   structuredClone(obj)
来源：http://pbr.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://ina.bbcook.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xli.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pap.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eac.jinqigfzy.top

[K06] 解析 URL 查询串
来源：http://aqy.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://niw.9152youxi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dfv.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bav.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mrc.uphjek.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ulw.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kfv.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vtg.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sby.cdnleiting.top

[K07] 进制转换
来源：http://omp.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ilz.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kne.jiagoushi.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cgd.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kyf.zhengqikj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://awc.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hij.chenzaomai.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bly.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vkp.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://qqx.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://zzm.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oxx.hammf.cn

JS:   v8.serialize(obj)        // Node
来源：http://hey.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://lgv.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ivu.zhongyouzk.top

Go:   encoding/gob
来源：http://xxy.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://yuu.quarkkingdee.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://evy.kuanghao11.cn

================================================================================
来源：http://lev.mhx1999.top

L. 网络请求
来源：http://yox.fehbvm.com

================================================================================
来源：http://ybb.jinqigufen.top

[L01] 发送 GET 请求
来源：http://uep.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uni.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yya.andypj.xyz

JS:   await fetch(url)
来源：http://dkm.yj20258.top

TS:   await fetch(url)
来源：http://gnr.ctjpmb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ypi.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://mby.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://riw.hywenlv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://erw.fehbvm.com

[L02] 发送 POST JSON
来源：http://lys.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://cqf.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://brt.yuxming.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rqw.shanyushiyangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zfb.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kzh.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hfr.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yzo.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oxr.yuxming.cn

[L03] 设置自定义请求头
来源：http://mks.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://udr.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yzi.jqgfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wxz.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fin.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lga.jinqigufen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yzg.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://heh.sysykeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nso.gotoacloud.top

[L04] 设置超时
来源：http://sdm.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://tzi.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xhs.gogol.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://crl.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://chs.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mlv.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qui.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dnt.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kaf.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://utk.bjfxy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jyl.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dxu.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nep.tarul.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://stn.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uho.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://soa.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jfl.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lep.pycfn.com

[L06] 解析响应为 JSON
来源：http://nsm.jinghuilouyu.cn

Py:   resp.json()
来源：http://anz.hesvh.cn

PHP:  json_decode($body, true);
来源：http://xfn.sweek.top

JS:   await resp.json()
来源：http://jcc.hongshengwenyu.top

TS:   await resp.json()
来源：http://gtq.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zrm.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wmk.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://jju.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hsq.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://nra.jinqigfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lzr.zhiwuduotai.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://swg.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://snh.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://ruk.sxryk.cn

Java: resp.statusCode()
来源：http://qsl.fktsv.cn

Go:   resp.StatusCode
来源：http://plc.cashguo.top

Ruby: resp.code.to_i
来源：http://axm.chenjidiqi.icu


<!-- 参考信息 -->