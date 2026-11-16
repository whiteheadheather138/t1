代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://lfa.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://koi.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://trq.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://exe.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hyg.zhoulong.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://jti.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tdc.gaohongyu789.top

[H10] 资源自动释放
来源：http://xjf.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://vtf.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yce.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://smz.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xuo.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aab.aibaodan.cn

Go:   defer f.Close()
来源：http://ltz.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hrp.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tvo.hfpthk.cn

================================================================================
来源：http://kas.yonumen.top

I. 正则表达式
来源：http://oww.ctjpmb.com

================================================================================
来源：http://mgr.sweek.top

[I01] 判断是否匹配
来源：http://uat.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xws.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://udz.nwbrower.top

JS:   /\d+/.test(s)
来源：http://ovd.jyoumei.cn

TS:   /\d+/.test(s)
来源：http://srn.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dxx.xylfe.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tre.jianghu66.top

Ruby: s.match?(/\d+/)
来源：http://uoz.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cvu.chenjidiqi.icu

[I02] 提取所有匹配
来源：http://iri.hysaishi.cn

Py:   re.findall(r"\d+", s)
来源：http://ecm.316326.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://brk.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lew.tanke756.top

TS:   s.match(/\d+/g)
来源：http://eun.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xil.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vgu.fanxiaobao.xyz

Ruby: s.scan(/\d+/)
来源：http://fgl.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://idc.yueranfly.top

[I03] 提取捕获分组
来源：http://jwb.sweek.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ffg.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cro.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qmj.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wjw.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bmb.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mse.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nmz.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yjq.cucudq.cn

[I04] 正则替换
来源：http://vds.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ccc.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://duf.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://zgv.cqqwz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://seu.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://nsg.andypj.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://yas.iojbl.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sje.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nop.jlsjyb.cn

[I05] 按正则拆分
来源：http://mqe.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hpk.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ger.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://mjf.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://bly.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://dvm.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qxn.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rtn.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iwe.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rmj.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ftr.nanxinkj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cer.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ilu.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rss.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rtz.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xsw.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gzb.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dqw.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://gel.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xfv.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ehh.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://apl.hnxiangtu.top

TS:   /error/gim
来源：http://sff.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ate.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rxl.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://lue.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bul.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://voe.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ohw.yongpay.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rvx.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uxd.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mik.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fli.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cde.ppjwa.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zko.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pqs.jlsjyb.cn

================================================================================
来源：http://uar.yuanzhike.top

J. 日期与时间
来源：http://bfk.ppjwa.cn

================================================================================
来源：http://jni.aibaodan.cn

[J01] 获取当前时间
来源：http://wfm.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pjs.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://seu.xziqi.cn

JS:   new Date();  Date.now()
来源：http://xiz.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://sjf.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tln.zdqjudy.top

Go:   time.Now()
来源：http://vpj.meibo888.top

Ruby: Time.now
来源：http://yms.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://avd.xylfe.cn

[J02] 格式化输出
来源：http://ccw.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pcu.epnwcf.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oim.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hpr.zhixingplan.top

TS:   d.toISOString()
来源：http://tcs.smart0.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yqp.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vho.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xxa.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lmu.snrcjt.cn

[J03] 字符串解析为日期
来源：http://xld.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kfu.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gqk.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://vlw.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://trb.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://jxe.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gyv.quarkkingdee.top

Ruby: Date.parse("2024-01-02")
来源：http://wpy.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fkk.yueranfly.top

[J04] 时间戳与日期互转
来源：http://cdw.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fbb.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://njz.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://usk.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zxb.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://djw.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dxf.xinyue.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yij.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kch.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://gnr.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://bhq.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://snk.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://thr.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ecc.jinqigfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://kwi.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zeo.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://ajp.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nhc.hnqzz.top

[J06] 计算两时间之差
来源：http://jvq.tarul.cn

Py:   (end - start).total_seconds()
来源：http://epb.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://owp.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://thu.jiagoushi.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dnz.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://rxk.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://egf.gaohongyu789.top

Ruby: end - start                 # 返回秒数
来源：http://jfu.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://eke.guowangkeji.top

[J07] 比较两个日期
来源：http://hcs.c1oappe.top

Py:   d1 < d2;  d1 == d2
来源：http://ksf.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zlt.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pmd.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://rki.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hjc.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oup.fzhhl.top

Ruby: d1 < d2;  d1 == d2
来源：http://vfg.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://frj.chenlongwang.top

[J08] 提取年月日与星期
来源：http://njm.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yzn.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ier.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://prf.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wlv.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sqb.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iew.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bvy.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dnn.hammf.cn

[J09] 时区处理
来源：http://rcd.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wrg.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fpx.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bkx.hywenlv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lxm.cheryme.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gwg.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://grs.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://alu.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nne.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://xka.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hxw.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jto.uphjek.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jps.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lnx.shanyushiyangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://foy.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nmo.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tpd.vqdsnc.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zon.zhijiandao.cn

================================================================================
来源：http://xsf.wangshuangyany.cn

K. JSON 与序列化
来源：http://lnf.kuanghao11.cn

================================================================================
来源：http://pes.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://zzt.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rqn.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://shl.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://pha.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://yfv.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pwj.birdmap.top

Go:   json.Marshal(obj)
来源：http://pkv.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://voz.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vud.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://crx.epnwcf.com

Py:   json.loads(s)
来源：http://wah.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://poo.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://auc.hnqzz.top

TS:   JSON.parse(s)
来源：http://dvv.52xcode.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zxd.cdnleiting.top

Go:   json.Unmarshal(data, &v)
来源：http://drh.sxryk.cn

Ruby: JSON.parse(s)
来源：http://wiq.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vou.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://oee.epnwcf.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://owe.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vxh.iojbl.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hfw.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jsi.zhijiandao.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cek.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vvq.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cbe.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://itt.yueranfly.top

[K04] 读取 JSON 文件
来源：http://npw.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gvk.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bnb.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dsi.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vrb.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gvr.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iox.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mmc.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qqb.sxryk.cn

[K05] 深拷贝对象
来源：http://wug.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://ojq.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://wcr.jianghu66.top

JS:   structuredClone(obj)
来源：http://lgu.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://rqe.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nto.zhengqikj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fay.ybcxt.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://phf.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ijl.c1oappe.top

[K06] 解析 URL 查询串
来源：http://drb.fanxiaobao.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hzs.birdmap.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cyg.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sfc.pycfn.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hwv.smart0.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sfl.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://dnp.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bdd.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rqy.xylfe.cn

[K07] 进制转换
来源：http://hwr.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bte.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kyx.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kds.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jvh.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://klb.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kub.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ztb.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mfc.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://qjj.pycfn.com

Py:   pickle.dumps(obj)
来源：http://qkg.hfpthk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yxb.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://kld.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://emk.mhx1999.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wgs.xylfe.cn

Go:   encoding/gob
来源：http://ihm.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://ikm.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wag.hywenlv.cn

================================================================================
来源：http://gkm.nanxinkj.top

L. 网络请求
来源：http://vpy.feifeiyinyue.top

================================================================================
来源：http://lxw.aibaodan.cn

[L01] 发送 GET 请求
来源：http://umr.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://czo.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tnw.yuanzhike.top

JS:   await fetch(url)
来源：http://slc.hysaishi.cn

TS:   await fetch(url)
来源：http://qwi.hammf.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://btn.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://nbc.nwbrower.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kmt.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qzh.yanxiufei.cn

[L02] 发送 POST JSON
来源：http://qan.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://ggk.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tsl.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qwq.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ivu.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qyy.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wes.jyoumei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hgw.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jxq.jianghu66.top

[L03] 设置自定义请求头
来源：http://erb.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jtx.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://crf.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cdn.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qfn.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://psm.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pcu.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://voo.jqgufenzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xyg.yanxiufei.cn

[L04] 设置超时
来源：http://gyx.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://vqn.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gud.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hkn.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uqa.ywan-chungtsiang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://msr.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wge.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://exy.cucudq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kcd.yj20258888.top

[L05] 上传文件（multipart）
来源：http://dsd.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wsi.meibo888.top


<!-- 参考信息 -->