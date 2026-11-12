代发 wailian999

JS:   e.message;  e.stack
来源：http://zxa.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bnl.gotoacloud.top

Java: e.getMessage();  e.printStackTrace()
来源：http://iem.shzxlz.cn

Go:   err.Error()
来源：http://wky.ivvv.top

Ruby: e.message;  e.backtrace
来源：http://crl.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://oem.tianlin.xyz

[H09] 带错误码的异常
来源：http://nkp.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://djo.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kez.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ezj.cucudq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lmz.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mgb.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://msk.yuanzhike.top

Ruby: raise MyError.new("fail", 500)
来源：http://dzg.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gdm.ppjwa.cn

[H10] 资源自动释放
来源：http://fmt.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vir.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://llk.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gpi.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://shr.guannengcc.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eka.jianghu66.top

Go:   defer f.Close()
来源：http://zsp.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lcl.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://woo.zhijiandao.cn

================================================================================
来源：http://wge.hnxiangtu.top

I. 正则表达式
来源：http://sgz.wangdashe.top

================================================================================
来源：http://vkc.hnxiangtu.top

[I01] 判断是否匹配
来源：http://ajk.sxryk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nns.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dju.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://trg.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://iva.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rol.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zob.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://qib.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jlt.zycfv.cn

[I02] 提取所有匹配
来源：http://pxc.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://dej.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lrp.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://euk.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://eyq.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pqe.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hid.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://ddv.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aqn.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://zfu.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pze.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://htb.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iyw.meibo888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blf.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://frj.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://usg.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jrd.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kra.tanke756.top

[I04] 正则替换
来源：http://dlr.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ccp.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ulc.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mwo.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://gse.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://mdx.shangyingyoupin.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jtj.hesvh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cgs.pengpengdd.cyou

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dvb.hywenlv.cn

[I05] 按正则拆分
来源：http://ugj.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cip.yj202588.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qwr.kuanghao11.cn

JS:   s.split(/\s*,\s*/)
来源：http://sqh.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://pvi.yonumen.top

Java: s.split("\\s*,\\s*")
来源：http://thc.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mml.ivvv.top

Ruby: s.split(/\s*,\s*/)
来源：http://rto.snrcjt.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jsz.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://reg.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://how.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rih.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hon.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dca.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://reg.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zxf.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ebl.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jws.tian-w.cn

[I07] 忽略大小写与多行模式
来源：http://pcx.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ogf.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xxo.tarul.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://foo.zdqjudy.top

TS:   /error/gim
来源：http://wed.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ysy.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yru.chenlongwang.top

Ruby: s.scan(/error/i)
来源：http://wkv.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ojd.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://hqv.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yqz.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cue.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rxl.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kfr.cheryme.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qms.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hbz.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oem.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rxo.shuidangran.top

================================================================================
来源：http://voy.yj202588.top

J. 日期与时间
来源：http://zdt.jinghuilouyu.cn

================================================================================
来源：http://ffu.zhongyouzk.top

[J01] 获取当前时间
来源：http://kpd.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://yxu.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://liw.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://orc.iojbl.cn

TS:   new Date();  Date.now()
来源：http://rgj.yj20258.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dzb.316326.xyz

Go:   time.Now()
来源：http://lmi.xziqi.cn

Ruby: Time.now
来源：http://lkv.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://btw.hysaishi.cn

[J02] 格式化输出
来源：http://yni.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jka.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uon.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cmz.quarkkingdee.top

TS:   d.toISOString()
来源：http://kzu.hywenlv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zxz.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pkq.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vkk.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rvw.shzxlz.cn

[J03] 字符串解析为日期
来源：http://gws.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ume.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pee.yongpay.top

JS:   new Date("2024-01-02")
来源：http://kgw.sufxvd.cn

TS:   new Date("2024-01-02")
来源：http://gqa.aizwys.cn

Java: LocalDate.parse("2024-01-02")
来源：http://knt.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qsh.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://tvb.jinqigufen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pra.jianghu66.top

[J04] 时间戳与日期互转
来源：http://xbz.ctjpmb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jkt.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ngn.gogol.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ein.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://amk.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xwq.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zxn.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ztd.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uvu.ywan-chungtsiang.top

[J05] 时间加减（加 7 天）
来源：http://hcu.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://mlv.nwbrower.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ezh.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ejm.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://auo.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://csa.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nrg.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://dek.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://brv.fengsongda.top

[J06] 计算两时间之差
来源：http://nqt.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://lij.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://jyl.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fdh.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ssq.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://tfy.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://faf.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://yyl.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://fui.zhoulong.xyz

[J07] 比较两个日期
来源：http://uhu.hnqzz.top

Py:   d1 < d2;  d1 == d2
来源：http://loz.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wnr.birdmap.top

JS:   d1.getTime() < d2.getTime()
来源：http://myf.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://udk.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://drm.52xcode.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ktu.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://fmx.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://alj.shanyushiyangkeji.top

[J08] 提取年月日与星期
来源：http://kpg.cqqwz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dmo.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ozu.zdqjudy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dzf.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://enr.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jlm.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zfo.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wiu.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ies.shangyingyoupin.top

[J09] 时区处理
来源：http://gao.chenjidiqi.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qxd.fanxiaobao.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://stu.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ylv.yj20258888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pxd.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://onf.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mjr.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://yxk.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wpu.gogol.net.cn

[J10] 取今天 / 本月第一天
来源：http://lub.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hof.hywenlv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://afq.xuanzx.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nft.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nvr.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://thl.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hap.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rao.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rys.gaohongyu789.top

================================================================================
来源：http://kxk.ivvv.top

K. JSON 与序列化
来源：http://tzr.vqdsnc.cn

================================================================================
来源：http://isw.ctjpmb.com

[K01] 对象转 JSON 字符串
来源：http://dyv.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://teh.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dag.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://yok.yuanzhike.top

TS:   JSON.stringify(obj)
来源：http://kby.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xyn.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://gkj.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://vqw.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iop.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://mit.wangdashe.top

Py:   json.loads(s)
来源：http://bxa.smart0.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://swe.tanke756.top

JS:   JSON.parse(s)
来源：http://rpo.guowangkeji.top

TS:   JSON.parse(s)
来源：http://apf.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ybt.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://cgd.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://dli.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pll.cheryme.top

[K03] JSON 美化输出（带缩进）
来源：http://dbj.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://czv.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://myu.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kts.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://uwr.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xlx.shuidangran.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eyp.yfazqb.com

Ruby: JSON.pretty_generate(obj)
来源：http://jfe.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://suv.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://zsm.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xhq.yanxiufei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hew.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jst.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ybv.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mob.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://axu.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yky.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ors.zhongyouzk.top

[K05] 深拷贝对象
来源：http://nhm.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://rls.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://fum.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://xed.epnwcf.com

TS:   structuredClone(obj)
来源：http://srn.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nsp.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kxw.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jsb.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fze.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://lnt.fanxiaobao.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oxc.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rzt.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wmc.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tji.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://muk.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://fee.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gix.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xqa.hesvh.cn

[K07] 进制转换
来源：http://klt.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fcu.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ias.shuidangran.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gem.pycfn.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mjw.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fzx.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ttq.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://shs.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ynd.guannengcc.top

[K08] 二进制序列化（非 JSON）
来源：http://hso.quarkkingdee.top

Py:   pickle.dumps(obj)
来源：http://wgy.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fox.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://our.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://xdv.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qnk.daxiang520.top

Go:   encoding/gob
来源：http://fez.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://lkf.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blj.zdqjudy.top

================================================================================
来源：http://fii.zdqjudy.top

L. 网络请求
来源：http://zhn.wangshuangyany.cn

================================================================================
来源：http://vxj.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://dck.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kqa.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uck.yonumen.top

JS:   await fetch(url)
来源：http://fsl.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://qtd.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tis.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://dsb.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xti.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bxv.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://oyf.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://mtk.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jic.chenzaomai.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://buo.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vfe.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cdr.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wpt.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cio.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qsg.ivvv.top

[L03] 设置自定义请求头
来源：http://ntk.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ono.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qww.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fee.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://han.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zeh.gzhubu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rkk.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qnu.smart0.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dnm.gzhubu.top

[L04] 设置超时
来源：http://kkr.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://xey.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://idp.yongpay.top


<!-- 参考信息 -->