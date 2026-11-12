代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rlw.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://lel.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ine.shuidangran.top

[H10] 资源自动释放
来源：http://tnq.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://gjx.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rrn.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zmz.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qhj.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gbd.zdqjudy.top

Go:   defer f.Close()
来源：http://bcd.c1oappe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://stn.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ngq.xuetiantiany.cn

================================================================================
来源：http://otx.redwolf501.top

I. 正则表达式
来源：http://jqz.meibo888.top

================================================================================
来源：http://kco.sjlbkw.cn

[I01] 判断是否匹配
来源：http://mib.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://slr.fengsongda.top

PHP:  preg_match('/\d+/', $s);
来源：http://lzi.sxryk.cn

JS:   /\d+/.test(s)
来源：http://hdo.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://gtk.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lud.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bqn.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://yrx.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kmi.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://lwi.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://exo.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fww.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zqm.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://pdg.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eoa.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://stp.jqgfzy.top

Ruby: s.scan(/\d+/)
来源：http://hxe.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fyh.xuetiantiany.cn

[I03] 提取捕获分组
来源：http://qhe.kuanghao11.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://clj.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tkv.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aai.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aoi.yanxiufei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://isu.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hhp.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mih.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vwh.daria6918.cn

[I04] 正则替换
来源：http://xcd.vehdjk.com

Py:   re.sub(r"\d+", "#", s)
来源：http://rbt.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oaw.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tmf.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://lkr.9152youxi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rrz.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://glr.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kho.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nli.hnqzz.top

[I05] 按正则拆分
来源：http://qxe.316326.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://lyb.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zsa.jlsjyb.cn

JS:   s.split(/\s*,\s*/)
来源：http://wdg.chenzaomai.com

TS:   s.split(/\s*,\s*/)
来源：http://qdw.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://kai.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pze.shangyingyoupin.top

Ruby: s.split(/\s*,\s*/)
来源：http://aar.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jdv.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gnj.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xph.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ccs.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oes.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lez.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://czj.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://swo.yuanzhike.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uud.pengpengdd.cyou

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cvl.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://azm.ppjwa.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vxd.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://znu.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qsx.hfpthk.cn

TS:   /error/gim
来源：http://rqn.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sxk.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://syc.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://avj.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ehx.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://mwg.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://efp.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lny.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kus.chenjidiqi.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://npe.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rzq.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sdj.bjfxy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xtd.zhijiandao.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ysf.zhixingplan.top

================================================================================
来源：http://qgh.guowangkeji.top

J. 日期与时间
来源：http://egj.guowangkeji.top

================================================================================
来源：http://but.shangyingyoupin.top

[J01] 获取当前时间
来源：http://icl.zhengqikj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fzv.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jqn.c1oappe.top

JS:   new Date();  Date.now()
来源：http://mxr.yuxming.cn

TS:   new Date();  Date.now()
来源：http://tck.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://epo.kuanghao11.cn

Go:   time.Now()
来源：http://zqb.wangdashe.top

Ruby: Time.now
来源：http://wta.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cve.yj20258888.top

[J02] 格式化输出
来源：http://cqe.xingfuxueyuan.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ncq.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tau.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jpx.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://nze.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://giw.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jha.dashuyun.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tja.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oaa.dianchejie.cn

[J03] 字符串解析为日期
来源：http://vtz.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pnu.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fkb.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://gav.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://eqr.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://ozi.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vgx.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://ths.9152youxi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oyj.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://deq.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xig.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wpn.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sts.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lfq.shuidangran.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://owu.daxiang520.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uqk.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://veh.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://coh.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://eao.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://jfa.hywenlv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jjy.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hhe.zdbjq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uuv.dashuyun.cn

Java: LocalDate.now().plusDays(7)
来源：http://ssi.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pfr.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://otq.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://ljd.0kj1m.cn

[J06] 计算两时间之差
来源：http://oss.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://cnd.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://jaf.nwbrower.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ydo.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wfo.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://evl.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://aub.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://zih.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://xeh.ywan-chungtsiang.top

[J07] 比较两个日期
来源：http://tvr.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://yzh.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yow.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://qpo.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oxz.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eac.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zre.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://cmp.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://ujz.guowangkeji.top

[J08] 提取年月日与星期
来源：http://ydo.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zew.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vma.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sio.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bnj.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yik.shuidangran.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://csw.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mtj.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gmo.hesvh.cn

[J09] 时区处理
来源：http://glw.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://afd.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lzc.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mle.guannengcc.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yyb.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pjq.hongshengwenyu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kvu.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://dop.tarul.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ygr.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://yex.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gll.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://och.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fzs.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fhz.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sxz.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cwk.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yht.nanxuanxn.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rcf.zhaomingkeji.xyz

================================================================================
来源：http://sqw.tanke756.top

K. JSON 与序列化
来源：http://wdz.zhoulong.xyz

================================================================================
来源：http://xdy.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://tpw.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://skq.chenzaomai.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://glo.yongpay.top

JS:   JSON.stringify(obj)
来源：http://qpg.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://cuh.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ldw.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://hfq.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://tsh.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fss.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://fgl.jlsjyb.cn

Py:   json.loads(s)
来源：http://zob.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lqy.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://rjc.chenjidiqi.icu

TS:   JSON.parse(s)
来源：http://bfo.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qhj.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://kmr.cdnleiting.top

Ruby: JSON.parse(s)
来源：http://myd.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cna.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://laz.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iyb.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://imv.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pjq.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xce.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rhb.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eib.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://prt.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wte.xuetiantiany.cn

[K04] 读取 JSON 文件
来源：http://zvz.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://efj.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xmc.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://beu.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tyr.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dsd.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mkt.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qhy.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://reg.gotoacloud.top

[K05] 深拷贝对象
来源：http://eil.meibo888.top

Py:   copy.deepcopy(obj)
来源：http://zmr.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://rxz.c1oappe.top

JS:   structuredClone(obj)
来源：http://alx.iojbl.cn

TS:   structuredClone(obj)
来源：http://flp.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://kjh.tarul.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gsx.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gwq.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nev.jyoumei.cn

[K06] 解析 URL 查询串
来源：http://kcp.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pda.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tmv.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qkz.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lom.yfazqb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://grm.fehbvm.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://dmm.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xsl.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fun.haohaochexian.top

[K07] 进制转换
来源：http://acp.nanxuanxn.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xux.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ulr.zhoulong.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hpt.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rfj.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jsw.jqgufenzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://avf.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qoi.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kvp.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://llr.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://xec.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pof.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://igl.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://kff.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qqy.hongshengwenyu.top

Go:   encoding/gob
来源：http://ddi.yvedp.cn

Ruby: Marshal.dump(obj)
来源：http://iyo.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://snd.yanxiufei.cn

================================================================================
来源：http://erv.guannengcc.top

L. 网络请求
来源：http://nab.pycfn.com

================================================================================
来源：http://cjh.jianghu66.top

[L01] 发送 GET 请求
来源：http://nvq.fanxiaobao.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jla.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gjg.fehbvm.com

JS:   await fetch(url)
来源：http://xvs.cashguo.top

TS:   await fetch(url)
来源：http://udh.zhijiandao.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kos.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://upu.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ebd.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vzt.gogol.net.cn

[L02] 发送 POST JSON
来源：http://ukg.tanke756.top

Py:   requests.post(url, json={"a": 1})
来源：http://ero.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://per.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cdf.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zqd.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://voa.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://evp.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rxc.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mlj.hysaishi.cn

[L03] 设置自定义请求头
来源：http://iov.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aoh.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uje.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fzx.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yeo.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zly.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kmd.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://npr.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wrn.cheryme.top

[L04] 设置超时
来源：http://zra.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://sde.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gbg.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://igf.yj202588.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tgl.jqgfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wvn.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sxr.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hiq.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xxi.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://rdy.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://woz.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hby.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pxs.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://svb.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vxi.shanyushiyangtech.top


<!-- 参考信息 -->