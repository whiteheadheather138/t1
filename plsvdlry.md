代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://vyv.xuanzx.com

C#:   e.Message;  e.StackTrace
来源：http://xtk.yanxiufei.cn

[H09] 带错误码的异常
来源：http://whd.daxiang520.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gwr.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gol.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gdt.9152youxi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xst.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ywe.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ssj.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://rgn.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://diz.vqdsnc.cn

[H10] 资源自动释放
来源：http://veq.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pzx.bbcook.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hiv.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ggf.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ihc.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jpo.shzxlz.cn

Go:   defer f.Close()
来源：http://xaj.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://djm.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zjz.hnxiangtu.top

================================================================================
来源：http://cao.jianghu66.top

I. 正则表达式
来源：http://ffa.jqgfzy.top

================================================================================
来源：http://lvq.quarkkingdee.top

[I01] 判断是否匹配
来源：http://uuc.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tsk.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://mdv.fzhhl.top

JS:   /\d+/.test(s)
来源：http://eft.smart0.xyz

TS:   /\d+/.test(s)
来源：http://ltm.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lzm.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vrl.jlsjyb.cn

Ruby: s.match?(/\d+/)
来源：http://fxk.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mvl.316326.xyz

[I02] 提取所有匹配
来源：http://jlo.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://qbx.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ent.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://waz.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://stq.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xwj.fehbvm.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zdg.xingfuxueyuan.xyz

Ruby: s.scan(/\d+/)
来源：http://qzh.yfazqb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fws.ctjpmb.com

[I03] 提取捕获分组
来源：http://asc.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vuh.bjfxy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ccy.zhoulong.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xyk.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pgj.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hwy.sxryk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://htt.sufxvd.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pns.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ewm.xinyue.icu

[I04] 正则替换
来源：http://chw.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://udl.daria6918.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uqe.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://ixg.vehdjk.com

TS:   s.replace(/\d+/g, "#")
来源：http://fag.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tnj.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://pbz.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dhe.yfazqb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aim.yueranfly.top

[I05] 按正则拆分
来源：http://wir.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xpk.bjfxy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gxk.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://lvy.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://htm.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://fan.daxiang520.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gnc.ydzc1.top

Ruby: s.split(/\s*,\s*/)
来源：http://vnl.c1oappe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lqb.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://evq.xylfe.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lxy.cheryme.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://geq.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kmd.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kpj.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vlk.quarkkingdee.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kce.yonumen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://adh.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fdi.tian-w.cn

[I07] 忽略大小写与多行模式
来源：http://bum.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jim.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hmb.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wdp.iojbl.cn

TS:   /error/gim
来源：http://vfz.vqdsnc.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ewc.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tuf.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://stb.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cpi.cqqwz.cn

[I08] 贪婪与非贪婪匹配
来源：http://cgv.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ebz.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sdf.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iop.fzhhl.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wkx.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://gzg.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iul.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xxb.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bcr.gogol.net.cn

================================================================================
来源：http://xhq.tianlin.xyz

J. 日期与时间
来源：http://syr.daxiang520.top

================================================================================
来源：http://rtr.gogol.net.cn

[J01] 获取当前时间
来源：http://bky.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xct.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://web.cucudq.cn

JS:   new Date();  Date.now()
来源：http://tbr.sxryk.cn

TS:   new Date();  Date.now()
来源：http://woi.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ihv.jqgfzy.top

Go:   time.Now()
来源：http://plu.zdbjq.cn

Ruby: Time.now
来源：http://iqu.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uni.mhx1999.top

[J02] 格式化输出
来源：http://iux.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zgh.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gsj.wangdashe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://psq.cqqwz.cn

TS:   d.toISOString()
来源：http://zya.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wsi.ybcxt.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bui.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://psy.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cnr.ctjpmb.com

[J03] 字符串解析为日期
来源：http://zaz.tian-w.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://isf.fengsongda.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qaq.cqqwz.cn

JS:   new Date("2024-01-02")
来源：http://shy.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://wkf.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://clu.ehwqpu.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aox.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://ckr.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fje.ydzc1.top

[J04] 时间戳与日期互转
来源：http://uzr.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mnj.yonumen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zmt.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://knp.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qrj.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lty.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vmj.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gca.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ptf.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://ecm.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://azp.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qrd.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ieu.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vhe.xuetiantiany.cn

Java: LocalDate.now().plusDays(7)
来源：http://xge.havefunace.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://izd.yueranfly.top

Ruby: Time.now + 7 * 86400
来源：http://zwp.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://fng.sxryk.cn

[J06] 计算两时间之差
来源：http://kor.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://yay.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://xgr.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vxx.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://njh.yangfankeji.com

Java: Duration.between(start, end).toSeconds()
来源：http://rpa.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://yot.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://vhn.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://tou.xuetiantiany.cn

[J07] 比较两个日期
来源：http://lpk.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://hxm.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pok.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sjm.fehbvm.com

TS:   d1.getTime() < d2.getTime()
来源：http://oid.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ekg.yj202588.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oln.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://wfr.jinqigufen.top

C#:   d1 < d2;  d1 == d2
来源：http://lzn.fehbvm.com

[J08] 提取年月日与星期
来源：http://vdw.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zbg.52xcode.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hua.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rnw.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jsl.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nfj.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ljn.cqqwz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zgx.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qcn.jinyuanbaomall.cn

[J09] 时区处理
来源：http://axe.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kcc.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hgc.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://omx.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gdo.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://spf.yj20258.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xpv.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vvg.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qwl.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://een.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://wxc.cashguo.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jsp.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vdg.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ffq.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hdk.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ynu.smart0.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xfi.redwolf501.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ute.zhongyouzk.top

================================================================================
来源：http://jas.jinqigfzy.top

K. JSON 与序列化
来源：http://cur.shuidangran.top

================================================================================
来源：http://zts.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://ofo.vqdsnc.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gus.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bus.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://ljc.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://div.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://omv.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://orr.gotoacloud.top

Ruby: obj.to_json                                     // require "json"
来源：http://cyr.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ywt.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://voj.c1oappe.top

Py:   json.loads(s)
来源：http://wxi.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tht.fzhhl.top

JS:   JSON.parse(s)
来源：http://iqm.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://jzn.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wey.snrcjt.cn

Go:   json.Unmarshal(data, &v)
来源：http://wfk.fzhhl.top

Ruby: JSON.parse(s)
来源：http://hnp.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://njg.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ajr.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dkn.yj20258888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jck.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dpn.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fph.cdnleiting.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vgh.zhongyouzk.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lsv.xylfe.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mrg.0kj1m.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fyc.hongshengwenyu.top

[K04] 读取 JSON 文件
来源：http://csn.yangfankeji.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zmd.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qsn.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ebd.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nta.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jbf.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://msd.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mwm.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ueb.jyoumei.cn

[K05] 深拷贝对象
来源：http://gln.shanyushiyangtech.top

Py:   copy.deepcopy(obj)
来源：http://abp.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://tvc.yonumen.top

JS:   structuredClone(obj)
来源：http://jre.birdmap.top

TS:   structuredClone(obj)
来源：http://hpy.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://uqb.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rzg.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ktb.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ksy.chenzaomai.com

[K06] 解析 URL 查询串
来源：http://joi.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://avv.fengsongda.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ugg.shanyushiyangtech.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://noa.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fnf.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fbq.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wwn.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ftv.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kro.pengpengdd.cyou

[K07] 进制转换
来源：http://mff.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tje.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kst.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uza.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kmx.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dnq.gzhubu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kvz.fehbvm.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cgm.nanxuanxn.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pzs.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://ohx.ppjwa.cn

Py:   pickle.dumps(obj)
来源：http://cbg.ppjwa.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bly.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://omc.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://jde.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ser.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://mvd.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://rty.ybcxt.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jlf.cashguo.top

================================================================================
来源：http://oxo.zycfv.cn

L. 网络请求
来源：http://jdw.shanyushiyangtech.top

================================================================================
来源：http://ddr.shzxlz.cn

[L01] 发送 GET 请求
来源：http://yai.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://njl.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://beu.gaohongyu789.top

JS:   await fetch(url)
来源：http://klv.feifeiyinyue.top

TS:   await fetch(url)
来源：http://lye.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wng.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://tks.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mwt.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qkv.316326.xyz

[L02] 发送 POST JSON
来源：http://ewf.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://rvm.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rrx.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nzg.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bon.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nio.cqqwz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kvk.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xic.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blx.dianchejie.cn

[L03] 设置自定义请求头
来源：http://gnp.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ity.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mxj.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fxp.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oxu.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xbg.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tca.vehdjk.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cyn.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fpt.xylfe.cn

[L04] 设置超时
来源：http://zav.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://ebd.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://abn.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kvv.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gxh.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hoj.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://edw.zhiwuduotai.top


<!-- 参考信息 -->