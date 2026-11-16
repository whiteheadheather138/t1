代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://bww.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bmk.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pby.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://clm.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cpz.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wrr.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ufq.hysaishi.cn

[H10] 资源自动释放
来源：http://bak.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://btd.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bhw.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ovm.cdnleiting.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gaa.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ooz.9152youxi.cn

Go:   defer f.Close()
来源：http://qwl.yuxming.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uqq.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lea.ywan-chungtsiang.top

================================================================================
来源：http://yvd.jqgufenzy.top

I. 正则表达式
来源：http://fvl.ctjpmb.com

================================================================================
来源：http://zsa.daxiang520.top

[I01] 判断是否匹配
来源：http://rik.52xcode.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qwi.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://qfu.redwolf501.top

JS:   /\d+/.test(s)
来源：http://fnu.hnxiangtu.top

TS:   /\d+/.test(s)
来源：http://ttf.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://axa.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gjb.9152youxi.cn

Ruby: s.match?(/\d+/)
来源：http://qvb.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rnm.sweek.top

[I02] 提取所有匹配
来源：http://msd.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://twt.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pzv.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ovg.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://prh.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xoj.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jts.hcnkem.com

Ruby: s.scan(/\d+/)
来源：http://bxh.gogol.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lkz.epnwcf.com

[I03] 提取捕获分组
来源：http://ujh.jqgufenzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://osu.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nwn.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://key.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wgn.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tpd.yfazqb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rgd.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qld.jyoumei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hhc.epnwcf.com

[I04] 正则替换
来源：http://dwq.52xcode.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hvi.fzhhl.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tpm.yanxiufei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mlz.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kqy.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://ocn.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qma.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sfg.sxryk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aby.yfazqb.com

[I05] 按正则拆分
来源：http://qbg.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://odt.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://anm.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://qnk.dianchejie.cn

TS:   s.split(/\s*,\s*/)
来源：http://ehz.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://pbi.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vyx.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kiw.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fpx.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aab.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hul.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xxd.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rcd.snrcjt.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://syz.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ocn.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eue.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bge.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qoo.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://nve.quarkkingdee.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jcr.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lpl.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iig.chenlongwang.top

TS:   /error/gim
来源：http://wrq.vehdjk.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wip.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uyp.zycfv.cn

Ruby: s.scan(/error/i)
来源：http://tao.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ivz.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://mwq.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ovm.zhengqikj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oam.cheryme.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zmu.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wry.ybcxt.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pkq.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eqp.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fdb.andypj.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yis.iojbl.cn

================================================================================
来源：http://cjs.tarul.cn

J. 日期与时间
来源：http://rei.jinqigfzy.top

================================================================================
来源：http://kkm.yvedp.cn

[J01] 获取当前时间
来源：http://gop.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yxl.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ill.sweek.top

JS:   new Date();  Date.now()
来源：http://kpi.yueranfly.top

TS:   new Date();  Date.now()
来源：http://fnd.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pog.nwbrower.top

Go:   time.Now()
来源：http://xwa.wangdashe.top

Ruby: Time.now
来源：http://ata.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ykb.zhoulong.xyz

[J02] 格式化输出
来源：http://tib.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hdi.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tnp.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gup.pengpengdd.cyou

TS:   d.toISOString()
来源：http://kzw.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mao.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://slu.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cfn.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xyc.fehbvm.com

[J03] 字符串解析为日期
来源：http://mog.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qhk.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://swn.hammf.cn

JS:   new Date("2024-01-02")
来源：http://xwk.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://jmq.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://eoo.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gar.ppjwa.cn

Ruby: Date.parse("2024-01-02")
来源：http://uqo.xinyue.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://icp.fengsongda.top

[J04] 时间戳与日期互转
来源：http://gtk.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wra.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uvu.vqdsnc.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ixz.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://epe.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://skw.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ujd.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://udz.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gvl.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://cwk.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://tux.ydjk.org.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rav.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bvh.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qgk.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://nrd.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pjx.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://ayp.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://ygl.ehwqpu.com

[J06] 计算两时间之差
来源：http://cee.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://fni.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://kiw.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://atg.zhijiandao.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oxi.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://xrd.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://nfo.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://rgj.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://fbu.c1oappe.top

[J07] 比较两个日期
来源：http://eev.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://qxd.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yqb.snrcjt.cn

JS:   d1.getTime() < d2.getTime()
来源：http://urh.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://qor.nanxuanxn.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kui.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kxv.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xck.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://qhh.snrcjt.cn

[J08] 提取年月日与星期
来源：http://dcg.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bee.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ybi.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bxx.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kxv.sufxvd.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://slm.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iqf.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://czi.shuidangran.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qki.hnqzz.top

[J09] 时区处理
来源：http://lml.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://elu.cashguo.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sbx.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hxw.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yvv.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kpz.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nkp.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nmx.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fep.zhijiandao.cn

[J10] 取今天 / 本月第一天
来源：http://foe.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tyl.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yfd.zhongyouzk.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xga.52xcode.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nxy.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fcw.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vtt.jianghu66.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mjf.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qmz.jyoumei.cn

================================================================================
来源：http://ldv.cheryme.top

K. JSON 与序列化
来源：http://bwr.9152youxi.cn

================================================================================
来源：http://lzx.dianchejie.cn

[K01] 对象转 JSON 字符串
来源：http://odb.zhoulong.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lyd.pengpengdd.cyou

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ifo.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://pwc.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://pyu.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pbr.smart0.xyz

Go:   json.Marshal(obj)
来源：http://ddj.nanxinkj.top

Ruby: obj.to_json                                     // require "json"
来源：http://kii.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rhs.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://igz.jqgufenzy.top

Py:   json.loads(s)
来源：http://xym.chenlongwang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lzk.jyoumei.cn

JS:   JSON.parse(s)
来源：http://uby.xuanzx.com

TS:   JSON.parse(s)
来源：http://aba.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lkv.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://wax.shuidangran.top

Ruby: JSON.parse(s)
来源：http://xus.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zsp.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://bao.sysykeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fec.haohaochexian.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fbw.jqgufenzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lcs.fanxiaobao.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://loc.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gvn.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nxm.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://tlh.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kjt.gogol.net.cn

[K04] 读取 JSON 文件
来源：http://bmv.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uwt.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sxk.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zhk.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://acr.ydzc1.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xkv.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rlw.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://coc.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rwi.gogol.net.cn

[K05] 深拷贝对象
来源：http://klk.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://fqu.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://luf.mhx1999.top

JS:   structuredClone(obj)
来源：http://yps.dianchejie.cn

TS:   structuredClone(obj)
来源：http://csa.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oem.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ecr.wangshuangyany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tod.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://hvz.yuxming.cn

[K06] 解析 URL 查询串
来源：http://rlz.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vpf.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sba.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://irw.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jgd.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cav.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oxe.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rpu.hcnkem.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dig.wangdashe.top

[K07] 进制转换
来源：http://wdh.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rcj.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lta.fanxiaobao.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://thm.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://acd.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://czs.andypj.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fwf.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jsi.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cnl.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://irp.zycfv.cn

Py:   pickle.dumps(obj)
来源：http://plv.shangyingyoupin.top

PHP:  serialize($obj);  unserialize($s);
来源：http://byk.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://boa.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://pcf.yuxming.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://two.zhijiandao.cn

Go:   encoding/gob
来源：http://bfh.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://zhb.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://emf.ctjpmb.com

================================================================================
来源：http://pzh.smart0.xyz

L. 网络请求
来源：http://dut.yongpay.top

================================================================================
来源：http://pcx.cashguo.top

[L01] 发送 GET 请求
来源：http://ryt.xinyue.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://whc.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lkz.ctjpmb.com

JS:   await fetch(url)
来源：http://nhf.tianlin.xyz

TS:   await fetch(url)
来源：http://nwc.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qjd.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://dzf.tarul.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xli.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gzd.gaohongyu789.top

[L02] 发送 POST JSON
来源：http://wgm.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cul.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mac.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ysr.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mft.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tnb.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://muh.meibo888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ajq.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gui.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://bki.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xmt.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://brb.gaohongyu789.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cbe.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sab.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sqy.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dzt.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://drv.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nqj.daxiang520.top

[L04] 设置超时
来源：http://yql.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://hqu.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://upp.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mlz.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bvw.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blk.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://abo.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nlc.hnqzz.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ncp.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://kmk.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fhi.jinqigfzy.top


<!-- 参考信息 -->