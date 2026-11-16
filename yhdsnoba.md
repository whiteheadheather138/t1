代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://phi.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://odd.yj202588.top

[H09] 带错误码的异常
来源：http://dsa.hammf.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pvw.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tzp.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hpa.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://opl.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hsd.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://opg.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://gmi.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gbs.c1oappe.top

[H10] 资源自动释放
来源：http://bzh.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://jbo.sxryk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pya.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ylh.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://htm.52xcode.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nks.ybcxt.top

Go:   defer f.Close()
来源：http://euk.fanxiaobao.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hjf.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://exi.bjfxy.top

================================================================================
来源：http://pwr.cqqwz.cn

I. 正则表达式
来源：http://uwy.yj20258888.top

================================================================================
来源：http://whp.dashuyun.cn

[I01] 判断是否匹配
来源：http://ewh.sufxvd.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pmm.redwolf501.top

PHP:  preg_match('/\d+/', $s);
来源：http://uya.ybcxt.top

JS:   /\d+/.test(s)
来源：http://ktl.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://vvv.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ydw.316326.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lxb.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://jsj.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jhq.shuidangran.top

[I02] 提取所有匹配
来源：http://ziy.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://rxg.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ffg.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kjr.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://way.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yiy.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oiq.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://jpa.iojbl.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://emh.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://ycx.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yil.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gce.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://and.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bnj.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rer.jinqigufen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yam.cashguo.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bfs.tianlin.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vbm.yuxming.cn

[I04] 正则替换
来源：http://znb.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aws.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rqd.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ihe.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://scs.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://ema.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mad.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lzu.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zwm.zycfv.cn

[I05] 按正则拆分
来源：http://ehd.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://riy.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mpm.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://elv.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://yyl.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://bjf.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iim.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://uuy.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pmi.sjlbkw.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zhi.cheryme.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ttl.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hki.yuanzhike.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dpn.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jdw.ybcxt.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://khf.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fmh.jinyuanbaomall.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dqz.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ora.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://rkv.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jqs.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ond.vqdsnc.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ylj.ydzc1.top

TS:   /error/gim
来源：http://tni.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ktb.chenjidiqi.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jnx.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://ict.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vez.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://aov.chenjidiqi.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jnt.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ypv.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://elu.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rqu.hnqzz.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zfe.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hsp.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bva.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://liz.daxiang520.top

================================================================================
来源：http://rft.nwbrower.top

J. 日期与时间
来源：http://crt.uphjek.com

================================================================================
来源：http://csa.yvedp.cn

[J01] 获取当前时间
来源：http://ppe.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kow.gogol.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ppi.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://wjz.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://xse.ywan-chungtsiang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dsw.ydjk.org.cn

Go:   time.Now()
来源：http://rjr.ivvv.top

Ruby: Time.now
来源：http://cby.zhiwuduotai.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sec.ctjpmb.com

[J02] 格式化输出
来源：http://agp.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tvy.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://trs.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eew.yanxiufei.cn

TS:   d.toISOString()
来源：http://vkn.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://izi.sjlbkw.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bgf.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zhb.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://geo.uphjek.com

[J03] 字符串解析为日期
来源：http://xey.yj20258.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ozh.gzhubu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://odv.yvedp.cn

JS:   new Date("2024-01-02")
来源：http://vre.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://fyf.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bqc.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vml.bbcook.cn

Ruby: Date.parse("2024-01-02")
来源：http://sey.redwolf501.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://alo.xinyue.icu

[J04] 时间戳与日期互转
来源：http://dkx.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qrb.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qud.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ftc.dashuyun.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pic.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jux.jinghuilouyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mvo.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nsc.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xro.aizwys.cn

[J05] 时间加减（加 7 天）
来源：http://koo.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://agp.quarkkingdee.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jgo.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mbq.ydjk.org.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qut.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://jwr.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ltx.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://vqw.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://wjn.yuxming.cn

[J06] 计算两时间之差
来源：http://wib.ybcxt.top

Py:   (end - start).total_seconds()
来源：http://kth.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://koi.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xvk.vehdjk.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://doa.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://bjg.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://ika.yfazqb.com

Ruby: end - start                 # 返回秒数
来源：http://ztl.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://wfv.ydjk.org.cn

[J07] 比较两个日期
来源：http://dyh.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://oau.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mcv.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://loh.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://ocn.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ytb.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://inc.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://fzw.hysaishi.cn

C#:   d1 < d2;  d1 == d2
来源：http://zcs.jqgfzy.top

[J08] 提取年月日与星期
来源：http://amz.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gjy.ydjk.org.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pxk.xingfuxueyuan.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vwl.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nun.vehdjk.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xfn.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rfl.aibaodan.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jgn.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://obh.sxryk.cn

[J09] 时区处理
来源：http://hqx.pengpengdd.cyou

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dvl.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sqw.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vih.yueranfly.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mnz.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bns.fanxiaobao.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kfx.tianlin.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://thj.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zjb.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://flj.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uba.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://crv.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wtw.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://elx.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wca.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yzf.yongpay.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zgk.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://usa.fehbvm.com

================================================================================
来源：http://taw.shanyushiyangtech.top

K. JSON 与序列化
来源：http://msv.shangyingyoupin.top

================================================================================
来源：http://akm.wangdashe.top

[K01] 对象转 JSON 字符串
来源：http://nca.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hhi.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iol.yuxming.cn

JS:   JSON.stringify(obj)
来源：http://nkw.ydzc1.top

TS:   JSON.stringify(obj)
来源：http://xvp.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://whl.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://hfq.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hrw.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://oli.xinyue.icu

[K02] JSON 字符串转对象
来源：http://qre.nanxinkj.top

Py:   json.loads(s)
来源：http://nev.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://svx.meibo888.top

JS:   JSON.parse(s)
来源：http://vbs.yuanzhike.top

TS:   JSON.parse(s)
来源：http://shd.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://atp.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://wlt.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://psh.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nxg.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://tcg.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zbw.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://een.zhoulong.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://nzp.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cbe.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://est.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hgt.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://xsu.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uea.hcnkem.com

[K04] 读取 JSON 文件
来源：http://ppv.ywan-chungtsiang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lvy.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://noa.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mqz.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wfq.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://txf.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://abn.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ijz.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zpp.redwolf501.top

[K05] 深拷贝对象
来源：http://jym.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://ftj.zhiwuduotai.top

PHP:  unserialize(serialize($obj));
来源：http://exv.dianchejie.cn

JS:   structuredClone(obj)
来源：http://xkw.shuidangran.top

TS:   structuredClone(obj)
来源：http://iig.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rkq.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uaf.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bjz.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kpe.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://tir.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oct.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nau.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vbc.cqqwz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ivx.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rqh.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kpw.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nmj.havefunace.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ryl.vehdjk.com

[K07] 进制转换
来源：http://sqa.sysykeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yif.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hbc.tanke756.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bzy.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ahj.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vux.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bnj.snrcjt.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rrx.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yjv.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://usy.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://eun.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cdb.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://lbd.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://gyx.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://slv.feifeiyinyue.top

Go:   encoding/gob
来源：http://kvu.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://jfp.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dex.fanxiaobao.xyz

================================================================================
来源：http://qez.9152youxi.cn

L. 网络请求
来源：http://oyv.ywan-chungtsiang.top

================================================================================
来源：http://ckx.hysaishi.cn

[L01] 发送 GET 请求
来源：http://ong.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dpo.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kou.dashuyun.cn

JS:   await fetch(url)
来源：http://jfp.yj20258888.top

TS:   await fetch(url)
来源：http://tjh.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uwa.c1oappe.top

Go:   resp, err := http.Get(url)
来源：http://afh.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cbf.ehwqpu.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://szm.redwolf501.top

[L02] 发送 POST JSON
来源：http://kcd.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://rmn.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bwx.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dso.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ydm.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://osj.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gjb.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tll.hesvh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tjd.yongpay.top

[L03] 设置自定义请求头
来源：http://ilc.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uyn.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qzv.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aud.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ghl.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uit.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yyx.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iol.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vuv.hnxiangtu.top

[L04] 设置超时
来源：http://wxn.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://sio.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mas.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lmp.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rmh.hywenlv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oxc.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://acf.hfpthk.cn


<!-- 参考信息 -->