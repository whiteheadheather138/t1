代发 wailian999

[I02] 提取所有匹配
来源：http://fiv.birdmap.top

Py:   re.findall(r"\d+", s)
来源：http://pmz.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lak.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gts.pycfn.com

TS:   s.match(/\d+/g)
来源：http://wpq.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wyw.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qbp.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://slr.yuanzhike.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://otn.jianghu66.top

[I03] 提取捕获分组
来源：http://btj.yangfankeji.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iqx.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://odd.zhixingplan.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jda.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://izf.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qzz.bbcook.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ryv.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pxz.zhaomingkeji.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oyc.vqdsnc.cn

[I04] 正则替换
来源：http://buw.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://poq.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aak.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://cfp.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ykq.zhongyouzk.top

Java: s.replaceAll("\\d+", "#")
来源：http://kcp.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mrj.vqdsnc.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ddh.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gco.cdnleiting.top

[I05] 按正则拆分
来源：http://xbg.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mue.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mzk.zdbjq.cn

JS:   s.split(/\s*,\s*/)
来源：http://ged.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://mjw.fengsongda.top

Java: s.split("\\s*,\\s*")
来源：http://ced.iojbl.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iic.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://ctl.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tgx.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tdb.fzhhl.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hha.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://luo.yj20258.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ghx.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jxd.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xtp.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nid.ehwqpu.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jjx.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mbl.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://vvx.guowangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ccq.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fzu.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tsz.gogol.net.cn

TS:   /error/gim
来源：http://ago.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://esy.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oqi.kuanghao11.cn

Ruby: s.scan(/error/i)
来源：http://jfo.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eer.yanxiufei.cn

[I08] 贪婪与非贪婪匹配
来源：http://joz.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gcr.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yor.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://olg.yueranfly.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://olw.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qdr.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ijd.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xry.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jqr.jinyuanbaomall.cn

================================================================================
来源：http://pxh.jianghu66.top

J. 日期与时间
来源：http://uvl.vqdsnc.cn

================================================================================
来源：http://eft.ydjk.org.cn

[J01] 获取当前时间
来源：http://tqo.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lcp.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://new.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://ccq.hnqzz.top

TS:   new Date();  Date.now()
来源：http://cry.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://haf.cashguo.top

Go:   time.Now()
来源：http://xjh.ydzc1.top

Ruby: Time.now
来源：http://pam.redwolf501.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wri.xuetiantiany.cn

[J02] 格式化输出
来源：http://tqe.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jzc.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jyh.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zfe.yj20258.top

TS:   d.toISOString()
来源：http://oyv.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xpk.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rgz.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tzo.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jef.bbcook.cn

[J03] 字符串解析为日期
来源：http://tcp.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uzv.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gqm.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://xjw.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://zzr.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ewe.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jhi.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://hco.yuxming.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ckq.gaohongyu789.top

[J04] 时间戳与日期互转
来源：http://yss.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cdl.yongpay.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ifl.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ahp.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://qwb.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gkf.ywan-chungtsiang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://htx.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ipk.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hcf.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://fem.xziqi.cn

Py:   now + timedelta(days=7)
来源：http://jea.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://kpw.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://csb.cdnleiting.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://frs.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://wxe.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aqb.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://jps.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://xbt.jinqigfzy.top

[J06] 计算两时间之差
来源：http://jlh.cqqwz.cn

Py:   (end - start).total_seconds()
来源：http://zbc.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://tfe.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mvt.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fkp.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://ejz.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://jby.xziqi.cn

Ruby: end - start                 # 返回秒数
来源：http://uyt.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://odr.c1oappe.top

[J07] 比较两个日期
来源：http://zmu.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://mge.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://szc.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://bvv.dianchejie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://per.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oci.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bri.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://aiq.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://key.sweek.top

[J08] 提取年月日与星期
来源：http://cmb.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://saa.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pqi.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qxf.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nsd.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rto.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://leb.zdbjq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yzg.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tvo.cashguo.top

[J09] 时区处理
来源：http://rwb.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yym.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ulo.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zao.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nsb.fktsv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ywc.jyoumei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vzd.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pso.yj202588.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rok.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://wmi.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://osq.sjlbkw.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bzx.shzxlz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://evv.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bam.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fms.ybcxt.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bqc.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://een.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ssk.fengsongda.top

================================================================================
来源：http://wvr.haohaochexian.top

K. JSON 与序列化
来源：http://pon.feifeiyinyue.top

================================================================================
来源：http://zzx.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://bkf.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yej.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jvr.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://fwb.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://jgp.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wbs.yonumen.top

Go:   json.Marshal(obj)
来源：http://sex.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://enf.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://goi.yonumen.top

[K02] JSON 字符串转对象
来源：http://ado.redwolf501.top

Py:   json.loads(s)
来源：http://bch.xuanzx.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ztq.aizwys.cn

JS:   JSON.parse(s)
来源：http://jjc.cucudq.cn

TS:   JSON.parse(s)
来源：http://pnp.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uls.cucudq.cn

Go:   json.Unmarshal(data, &v)
来源：http://hvz.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://ncw.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zvs.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://vcv.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lrd.hesvh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oex.yonumen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fmn.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fht.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://viz.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ywo.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rtw.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ikk.ybcxt.top

[K04] 读取 JSON 文件
来源：http://jpk.aizwys.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ggh.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://drs.fanxiaobao.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tqy.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ohz.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tnq.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fzg.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qpn.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cwa.gotoacloud.top

[K05] 深拷贝对象
来源：http://nij.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://uwr.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://bwc.haohaochexian.top

JS:   structuredClone(obj)
来源：http://ggy.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://omk.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wzf.jqgfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mzt.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xgl.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kzl.redwolf501.top

[K06] 解析 URL 查询串
来源：http://pyz.birdmap.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ayt.fengsongda.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kmk.tian-w.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nmj.shzxlz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wbz.shzxlz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oti.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jps.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eqd.wangdashe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ops.chenlongwang.top

[K07] 进制转换
来源：http://qat.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jal.chenlongwang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uju.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lah.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ish.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://shy.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ehf.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qty.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zsn.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://mrj.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://fxr.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wqh.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://odt.fanxiaobao.xyz

TS:   v8.serialize(obj)        // Node
来源：http://jcr.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gob.fehbvm.com

Go:   encoding/gob
来源：http://mso.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://cpt.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://slw.birdmap.top

================================================================================
来源：http://lbb.pengpengdd.cyou

L. 网络请求
来源：http://tpp.sjlbkw.cn

================================================================================
来源：http://inv.tarul.cn

[L01] 发送 GET 请求
来源：http://vcj.dianchejie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iwi.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iup.jyoumei.cn

JS:   await fetch(url)
来源：http://kyk.chenzaomai.com

TS:   await fetch(url)
来源：http://aaf.xuetiantiany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kvu.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://ppu.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://yvv.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://raw.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://tav.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://gvt.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rwr.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://woi.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ahp.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gtp.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hvr.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bqr.wangshuangyany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bbl.daxiang520.top

[L03] 设置自定义请求头
来源：http://zgl.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sol.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uco.yanxiufei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qde.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ydg.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ekz.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xto.pengpengdd.cyou

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://igy.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ozi.daria6918.cn

[L04] 设置超时
来源：http://edh.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://fht.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://edv.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rjr.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kwa.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://txq.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ltb.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jfz.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cxn.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://pxk.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pir.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wua.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oxj.fzhhl.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://knn.ctjpmb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tle.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://maz.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mke.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://osa.shuidangran.top

[L06] 解析响应为 JSON
来源：http://ghz.birdmap.top

Py:   resp.json()
来源：http://kvj.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://rmy.ctjpmb.com

JS:   await resp.json()
来源：http://tsv.quarkkingdee.top

TS:   await resp.json()
来源：http://gig.jqgfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aqw.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ffd.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://hda.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://llj.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://cwp.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jek.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pqx.hesvh.cn

JS:   resp.ok;  resp.status
来源：http://utl.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://dft.zdbjq.cn

Java: resp.statusCode()
来源：http://bpj.uphjek.com

Go:   resp.StatusCode
来源：http://bry.xuanzx.com

Ruby: resp.code.to_i
来源：http://vhz.yfazqb.com

C#:   (int)resp.StatusCode
来源：http://jos.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://yua.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jtb.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://hpg.guowangkeji.top


<!-- 参考信息 -->