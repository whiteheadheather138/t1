代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://wss.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://jvs.aizwys.cn

Py:   str(e);  traceback.format_exc()
来源：http://hhp.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gbq.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://cqg.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vyg.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ens.zhongyouzk.top

Go:   err.Error()
来源：http://rna.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://lhr.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://fgu.cashguo.top

[H09] 带错误码的异常
来源：http://ieb.zycfv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vkp.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ytn.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://itf.tarul.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gmh.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wjc.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://seg.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qkf.hammf.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sua.yongpay.top

[H10] 资源自动释放
来源：http://dkp.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://anb.uphjek.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sch.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sta.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yux.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xpw.zhengqikj.top

Go:   defer f.Close()
来源：http://bpg.smart0.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hzb.9152youxi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jdk.daria6918.cn

================================================================================
来源：http://ror.zdqjudy.top

I. 正则表达式
来源：http://nyj.sysykeji.top

================================================================================
来源：http://gjz.jqgfzy.top

[I01] 判断是否匹配
来源：http://cqu.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hlk.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://azd.iojbl.cn

JS:   /\d+/.test(s)
来源：http://tss.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://ixy.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cho.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://njt.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://zyh.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://haq.52xcode.cn

[I02] 提取所有匹配
来源：http://tdn.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://aov.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tvw.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xja.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://hgc.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://khb.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ijn.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://awc.meibo888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tqn.jqgfzy.top

[I03] 提取捕获分组
来源：http://nfv.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kdc.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://igz.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vbr.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pkd.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dyd.fzhhl.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vas.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hep.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://luu.hcnkem.com

[I04] 正则替换
来源：http://xtz.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://exy.shzxlz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sxj.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xnd.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qxc.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wgr.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ipw.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dxq.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fbd.hnqzz.top

[I05] 按正则拆分
来源：http://twe.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://mxh.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bii.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://bek.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://yhv.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://fef.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blr.yuanzhike.top

Ruby: s.split(/\s*,\s*/)
来源：http://ioo.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qud.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qxs.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rtw.wangdashe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sip.9152youxi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bpi.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ahn.chenzaomai.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://irh.ybcxt.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://egz.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pvh.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://umx.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://ioc.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wnq.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rpw.hnqzz.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ipt.guannengcc.top

TS:   /error/gim
来源：http://nzw.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ihl.daxiang520.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cpf.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://whr.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://los.shzxlz.cn

[I08] 贪婪与非贪婪匹配
来源：http://dpb.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yiy.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://axn.bjfxy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://heb.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tpd.shanyushiyangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pmr.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wgh.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wli.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ioc.zhengqikj.top

================================================================================
来源：http://xsz.zhoulong.xyz

J. 日期与时间
来源：http://ecy.quarkkingdee.top

================================================================================
来源：http://jge.chenjidiqi.icu

[J01] 获取当前时间
来源：http://uwb.hnqzz.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cvz.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ima.guannengcc.top

JS:   new Date();  Date.now()
来源：http://frd.hcnkem.com

TS:   new Date();  Date.now()
来源：http://bmx.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://soq.fengsongda.top

Go:   time.Now()
来源：http://oro.yueranfly.top

Ruby: Time.now
来源：http://reg.shuidangran.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ors.cashguo.top

[J02] 格式化输出
来源：http://gpy.meibo888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yzm.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jwv.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://grx.ctjpmb.com

TS:   d.toISOString()
来源：http://rod.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zet.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mad.c1oappe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://auw.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nwx.daxiang520.top

[J03] 字符串解析为日期
来源：http://fpg.zhiwuduotai.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ije.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sfw.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://yem.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://jhs.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://bmd.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qfb.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://mgx.zhiwuduotai.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mya.sysykeji.top

[J04] 时间戳与日期互转
来源：http://owy.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://skp.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jya.yuanzhike.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dvy.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://sey.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bgp.c1oappe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wxo.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vot.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jqd.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://bfz.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://mdb.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://erk.shuidangran.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qca.cqqwz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pao.ywan-chungtsiang.top

Java: LocalDate.now().plusDays(7)
来源：http://ezm.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dli.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://teo.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://nks.bjfxy.top

[J06] 计算两时间之差
来源：http://vhx.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://xhb.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://drb.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://izq.bbcook.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jde.yanxiufei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bkj.bjfxy.top

Go:   end.Sub(start).Hours()
来源：http://dsl.gaohongyu789.top

Ruby: end - start                 # 返回秒数
来源：http://frm.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://fuh.kuanghao11.cn

[J07] 比较两个日期
来源：http://ybm.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://prm.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://exo.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://vfs.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://zxu.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://avy.vehdjk.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wsh.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://fgq.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://nvx.yuanzhike.top

[J08] 提取年月日与星期
来源：http://vqu.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://urc.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xwu.yfazqb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bsu.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ezk.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oeg.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dii.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://equ.shanyushiyangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://trw.jinqigufen.top

[J09] 时区处理
来源：http://hnb.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ibn.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://olx.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://acn.feifeiyinyue.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mmd.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yni.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jrb.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gmw.hywenlv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lch.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://itz.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zxq.shanyushiyangtech.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nyu.yfazqb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hcw.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bgy.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pti.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hlx.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rqq.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kxn.cqqwz.cn

================================================================================
来源：http://iav.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://xwd.ydjk.org.cn

================================================================================
来源：http://laz.ywan-chungtsiang.top

[K01] 对象转 JSON 字符串
来源：http://ipt.zhaomingkeji.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gao.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ydz.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://yui.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://uot.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fey.316326.xyz

Go:   json.Marshal(obj)
来源：http://pew.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://lef.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://hjh.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://fvs.yvedp.cn

Py:   json.loads(s)
来源：http://uvb.sufxvd.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lsy.zhongyouzk.top

JS:   JSON.parse(s)
来源：http://ppt.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://vad.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yrb.aizwys.cn

Go:   json.Unmarshal(data, &v)
来源：http://rbo.meibo888.top

Ruby: JSON.parse(s)
来源：http://jsi.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://krj.tianlin.xyz

[K03] JSON 美化输出（带缩进）
来源：http://xjd.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eph.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hqm.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qez.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mmx.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zvx.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cwe.daria6918.cn

Ruby: JSON.pretty_generate(obj)
来源：http://opj.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://weh.ydjk.org.cn

[K04] 读取 JSON 文件
来源：http://wst.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://axa.zhongyouzk.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ccu.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nth.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sup.dianchejie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://evs.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kxm.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cpe.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tjx.shuidangran.top

[K05] 深拷贝对象
来源：http://mpo.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://yps.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://rap.zycfv.cn

JS:   structuredClone(obj)
来源：http://hhv.gzhubu.top

TS:   structuredClone(obj)
来源：http://rry.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://plb.dianchejie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://swn.uphjek.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://osz.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tfg.yj20258888.top

[K06] 解析 URL 查询串
来源：http://snz.hesvh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cpf.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bpk.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mqx.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vld.tanke756.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lgg.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gso.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gvq.jiagoushi.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eyx.tarul.cn

[K07] 进制转换
来源：http://kes.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mcq.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dgz.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ppu.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://atk.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rxa.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zdj.yuxming.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sne.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bki.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://mro.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://pvd.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fwh.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://uau.fehbvm.com

TS:   v8.serialize(obj)        // Node
来源：http://jce.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ksm.shangyingyoupin.top

Go:   encoding/gob
来源：http://bbo.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://ief.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dts.yj202588.top

================================================================================
来源：http://vuc.zhaomingkeji.xyz

L. 网络请求
来源：http://bfw.gaohongyu789.top

================================================================================
来源：http://jcs.yvedp.cn

[L01] 发送 GET 请求
来源：http://gkd.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ygv.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tfv.xinyue.icu

JS:   await fetch(url)
来源：http://csi.dianchejie.cn

TS:   await fetch(url)
来源：http://jig.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tmd.chenlongwang.top

Go:   resp, err := http.Get(url)
来源：http://krb.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://toq.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zzb.vehdjk.com

[L02] 发送 POST JSON
来源：http://bxz.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://otg.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wrh.hywenlv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wjd.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rnp.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uan.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rot.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kva.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ihm.0kj1m.cn

[L03] 设置自定义请求头
来源：http://spp.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sce.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zqs.ctjpmb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zri.snrcjt.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cba.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tmv.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yvc.chenzaomai.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sht.shangyingyoupin.top


<!-- 参考信息 -->