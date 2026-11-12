代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://coe.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://euv.gotoacloud.top

JS:   /\d+/.test(s)
来源：http://slg.xylfe.cn

TS:   /\d+/.test(s)
来源：http://xiq.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jza.nwbrower.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ton.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://zbz.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yea.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://vde.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://emk.tianlin.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dge.uphjek.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://drm.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://wlg.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jrq.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lsd.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://qjo.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cok.daxiang520.top

[I03] 提取捕获分组
来源：http://dik.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mnn.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gbv.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mon.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://txm.yfazqb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://onr.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iiy.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ojt.havefunace.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gtu.shzxlz.cn

[I04] 正则替换
来源：http://ikj.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wqh.yuanzhike.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lbj.aizwys.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jbd.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://jti.bjfxy.top

Java: s.replaceAll("\\d+", "#")
来源：http://mfi.dianchejie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ocs.vehdjk.com

Ruby: s.gsub(/\d+/, "#")
来源：http://bdb.yj202588.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ijh.vehdjk.com

[I05] 按正则拆分
来源：http://tyf.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yfg.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jcp.zhaomingkeji.xyz

JS:   s.split(/\s*,\s*/)
来源：http://chl.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://lbs.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://brs.zhongyouzk.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aod.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://iqm.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jzh.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ere.tianlin.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fnl.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ieq.yvedp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qsf.zhiwuduotai.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ibt.aibaodan.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://urp.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bwp.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dxl.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://llb.yanxiufei.cn

[I07] 忽略大小写与多行模式
来源：http://wqo.nanxuanxn.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cxe.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jqs.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pbr.cqqwz.cn

TS:   /error/gim
来源：http://fuw.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jrl.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mqr.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://wyp.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dnj.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://wbd.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://olz.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://odu.zhijiandao.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yvl.xingfuxueyuan.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pgq.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://srf.nwbrower.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kio.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nqq.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lxa.xingfuxueyuan.xyz

================================================================================
来源：http://ett.tanke756.top

J. 日期与时间
来源：http://eih.ydzc1.top

================================================================================
来源：http://fqq.quarkkingdee.top

[J01] 获取当前时间
来源：http://yor.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ilf.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lzc.316326.xyz

JS:   new Date();  Date.now()
来源：http://xtl.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://ssq.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://oxy.zhaomingkeji.xyz

Go:   time.Now()
来源：http://rcp.havefunace.top

Ruby: Time.now
来源：http://aax.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pfi.yuanzhike.top

[J02] 格式化输出
来源：http://nmy.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mtx.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oxy.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qqu.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://peb.yj20258.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://knm.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://stq.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://srv.zhixingplan.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yuv.pycfn.com

[J03] 字符串解析为日期
来源：http://ski.gogol.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mpo.hcnkem.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hzy.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://sfw.hammf.cn

TS:   new Date("2024-01-02")
来源：http://yaa.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://xbe.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kvv.smart0.xyz

Ruby: Date.parse("2024-01-02")
来源：http://bgt.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://scf.snrcjt.cn

[J04] 时间戳与日期互转
来源：http://unl.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ewc.fengsongda.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uol.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fbx.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mcr.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qbz.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sqq.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iys.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rib.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://nid.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://paj.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rxb.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pzv.9152youxi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://atc.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://zqz.jiagoushi.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fpa.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://xwt.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ptz.yongpay.top

[J06] 计算两时间之差
来源：http://fof.zhoulong.xyz

Py:   (end - start).total_seconds()
来源：http://oak.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://cxi.epnwcf.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ftq.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sgg.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://nql.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://ffy.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://gub.jinghuilouyu.cn

C#:   (end - start).TotalSeconds
来源：http://mlz.ydjk.org.cn

[J07] 比较两个日期
来源：http://zho.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://uqv.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dvk.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://ygk.gogol.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zxk.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xce.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://owr.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://red.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://tuc.ybcxt.top

[J08] 提取年月日与星期
来源：http://upy.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bcx.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rks.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yda.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rzw.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xdl.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://svd.pengpengdd.cyou

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fjr.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xdo.guannengcc.top

[J09] 时区处理
来源：http://klz.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://orr.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ycm.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tkg.bbcook.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://adt.andypj.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://irg.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bkl.yuanzhike.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mzu.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gnj.ydjk.org.cn

[J10] 取今天 / 本月第一天
来源：http://jwe.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://jpl.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zre.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bxp.gogol.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://arf.ivvv.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cls.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://brl.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zkd.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://trb.guowangkeji.top

================================================================================
来源：http://vfb.jyoumei.cn

K. JSON 与序列化
来源：http://jkf.xylfe.cn

================================================================================
来源：http://pen.zhaomingkeji.xyz

[K01] 对象转 JSON 字符串
来源：http://xsa.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pll.cdnleiting.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aeo.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://xfq.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://pri.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xxx.daxiang520.top

Go:   json.Marshal(obj)
来源：http://itg.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://rqm.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://tfr.andypj.xyz

[K02] JSON 字符串转对象
来源：http://exx.tanke756.top

Py:   json.loads(s)
来源：http://npr.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://slv.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://nhw.chenjidiqi.icu

TS:   JSON.parse(s)
来源：http://fgo.zhijiandao.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lnb.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://vro.shzxlz.cn

Ruby: JSON.parse(s)
来源：http://uoz.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://deg.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://sex.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dry.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://duk.hesvh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cdg.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qit.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://toz.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kxj.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://oac.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zzr.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://dcx.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tsa.sweek.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ltn.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lqp.svipenyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://won.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://odj.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iim.hesvh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ees.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gsg.hammf.cn

[K05] 深拷贝对象
来源：http://fcy.cashguo.top

Py:   copy.deepcopy(obj)
来源：http://nlv.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://ryu.jianghu66.top

JS:   structuredClone(obj)
来源：http://mfl.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://pah.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://knh.dashuyun.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tzj.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fps.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vlv.c1oappe.top

[K06] 解析 URL 查询串
来源：http://pmt.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cmp.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://thn.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://enp.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tzx.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fdp.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uec.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vbi.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hok.tanke756.top

[K07] 进制转换
来源：http://ftv.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zyp.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vna.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ouo.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://azf.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cgx.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qka.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rlh.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://apr.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://neo.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://xlx.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://wrv.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://aka.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://ccu.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rlv.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://whs.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://ibh.ydzc1.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lde.jqgfzy.top

================================================================================
来源：http://zrz.sysykeji.top

L. 网络请求
来源：http://lvd.smart0.xyz

================================================================================
来源：http://ruz.haohaochexian.top

[L01] 发送 GET 请求
来源：http://qdu.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mko.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fdx.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://tqs.ehwqpu.com

TS:   await fetch(url)
来源：http://wlw.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gip.zhengqikj.top

Go:   resp, err := http.Get(url)
来源：http://wep.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://tqr.zhijiandao.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://alz.yongpay.top

[L02] 发送 POST JSON
来源：http://xdi.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://fkp.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gjh.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hyz.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mer.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xmg.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tzc.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pld.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fhy.dianchejie.cn

[L03] 设置自定义请求头
来源：http://dnp.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nmv.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tko.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lvw.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://woz.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ikh.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zxh.feifeiyinyue.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://flq.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cbe.tian-w.cn

[L04] 设置超时
来源：http://ksd.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://vaf.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dgl.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://whk.tanke756.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ukf.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ony.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jop.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qst.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pwr.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://hio.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vnc.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rsy.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tvm.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jcs.vqdsnc.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dvp.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://juc.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wfn.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bpd.nwbrower.top

[L06] 解析响应为 JSON
来源：http://vdc.wangdashe.top

Py:   resp.json()
来源：http://vii.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://yza.sxryk.cn

JS:   await resp.json()
来源：http://gtz.hywenlv.cn

TS:   await resp.json()
来源：http://swm.gaohongyu789.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vjs.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fot.shuidangran.top

Ruby: JSON.parse(resp.body)
来源：http://mjt.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qbt.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://xhn.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rrg.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ehw.hammf.cn

JS:   resp.ok;  resp.status
来源：http://abt.yongpay.top


<!-- 参考信息 -->