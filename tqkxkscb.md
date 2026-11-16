代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://dsw.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tut.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ihs.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jky.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nkr.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://rdb.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xkc.tian-w.cn

[H10] 资源自动释放
来源：http://ohu.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ywm.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://src.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zjp.quarkkingdee.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iax.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kya.mhx1999.top

Go:   defer f.Close()
来源：http://goq.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://woe.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://khd.zdqjudy.top

================================================================================
来源：http://kou.xuetiantiany.cn

I. 正则表达式
来源：http://uyq.jiagoushi.top

================================================================================
来源：http://fkg.shuidangran.top

[I01] 判断是否匹配
来源：http://ezw.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fvd.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://bia.shangyingyoupin.top

JS:   /\d+/.test(s)
来源：http://rio.ctjpmb.com

TS:   /\d+/.test(s)
来源：http://knu.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bgm.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mam.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://ipl.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://htc.zhixingplan.top

[I02] 提取所有匹配
来源：http://ckb.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://zxh.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vcy.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wur.iojbl.cn

TS:   s.match(/\d+/g)
来源：http://gha.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qlm.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ekr.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://igo.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://psn.smart0.xyz

[I03] 提取捕获分组
来源：http://lki.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ufd.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://peg.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zun.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://emw.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wpe.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gtt.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ogb.jinghuilouyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hyr.c1oappe.top

[I04] 正则替换
来源：http://frb.sufxvd.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://unj.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sup.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://xmn.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://imz.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iyl.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nxt.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gyd.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mjj.cheryme.top

[I05] 按正则拆分
来源：http://umf.tanke756.top

Py:   re.split(r"\s*,\s*", s)
来源：http://erp.zhiwuduotai.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lhr.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://bzb.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://foc.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://zsm.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oxt.xylfe.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vej.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tid.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dvd.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zhc.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ypz.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cfj.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xbq.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jqc.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rrm.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://phw.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mkm.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://oao.ctjpmb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gto.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tkf.jqgufenzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wxj.wangdashe.top

TS:   /error/gim
来源：http://dkb.xingfuxueyuan.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xec.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://puq.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://uhh.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://abb.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://and.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aax.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://miz.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://klf.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://unm.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lnb.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jvp.hfpthk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xqu.ppjwa.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yfd.feifeiyinyue.top

================================================================================
来源：http://gai.daxiang520.top

J. 日期与时间
来源：http://ufk.aibaodan.cn

================================================================================
来源：http://ucp.yj20258888.top

[J01] 获取当前时间
来源：http://aho.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://dpm.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uio.hesvh.cn

JS:   new Date();  Date.now()
来源：http://pyf.zdqjudy.top

TS:   new Date();  Date.now()
来源：http://eoh.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://huc.yj20258888.top

Go:   time.Now()
来源：http://okz.yongpay.top

Ruby: Time.now
来源：http://tzg.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oxb.fengsongda.top

[J02] 格式化输出
来源：http://ivw.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://czg.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gwv.cucudq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ody.feifeiyinyue.top

TS:   d.toISOString()
来源：http://igp.redwolf501.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ifg.bjfxy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tar.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hwf.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://raz.ybcxt.top

[J03] 字符串解析为日期
来源：http://rrx.zhaomingkeji.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zmf.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ktb.yuanzhike.top

JS:   new Date("2024-01-02")
来源：http://nfc.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://hvd.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://kze.zycfv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rqy.aibaodan.cn

Ruby: Date.parse("2024-01-02")
来源：http://bzh.shanyushiyangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ujs.yj20258888.top

[J04] 时间戳与日期互转
来源：http://xhy.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://igv.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fju.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kgp.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eqm.zhoulong.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gnc.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pmr.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eiq.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oww.hywenlv.cn

[J05] 时间加减（加 7 天）
来源：http://nkw.yongpay.top

Py:   now + timedelta(days=7)
来源：http://lex.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pbu.ydzc1.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rfp.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bwq.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://qby.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://der.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://hak.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hmh.redwolf501.top

[J06] 计算两时间之差
来源：http://kiv.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://naf.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://hdw.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uxt.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://btl.nanxinkj.top

Java: Duration.between(start, end).toSeconds()
来源：http://epc.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://mfs.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://viz.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://ftk.0kj1m.cn

[J07] 比较两个日期
来源：http://lqa.jinqigufen.top

Py:   d1 < d2;  d1 == d2
来源：http://kgp.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://byb.nwbrower.top

JS:   d1.getTime() < d2.getTime()
来源：http://pns.iojbl.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rif.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mma.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ltb.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://xrc.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://dix.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://qdy.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ktd.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xlp.pycfn.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cqd.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vhk.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ffy.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://exm.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ibv.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fxw.shanyushiyangtech.top

[J09] 时区处理
来源：http://niy.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://htm.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vvx.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ukb.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lzx.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eam.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vou.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kho.cucudq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://otz.hongshengwenyu.top

[J10] 取今天 / 本月第一天
来源：http://pqi.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sfc.xinyue.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kcu.yj20258888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jcl.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dvv.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hup.zhoulong.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xme.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ffo.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zjo.shanyushiyangtech.top

================================================================================
来源：http://wco.chenlongwang.top

K. JSON 与序列化
来源：http://ovw.iojbl.cn

================================================================================
来源：http://mxk.hfpthk.cn

[K01] 对象转 JSON 字符串
来源：http://ogo.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iqi.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qdl.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://rbk.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://fue.tianlin.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ino.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://ern.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://tpb.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kth.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://iwl.haohaochexian.top

Py:   json.loads(s)
来源：http://fst.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gdo.chenzaomai.com

JS:   JSON.parse(s)
来源：http://mqc.sufxvd.cn

TS:   JSON.parse(s)
来源：http://vvy.gotoacloud.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jhz.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://feu.nanxinkj.top

Ruby: JSON.parse(s)
来源：http://wic.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zjl.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://alu.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gsa.tianlin.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uur.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nku.cucudq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fxd.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mkc.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fwv.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://byt.iojbl.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wyn.xuetiantiany.cn

[K04] 读取 JSON 文件
来源：http://byr.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://txp.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xyx.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kma.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://upu.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ydg.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://grt.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ttp.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ztq.yj20258888.top

[K05] 深拷贝对象
来源：http://iqv.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://gah.svipenyu.cn

PHP:  unserialize(serialize($obj));
来源：http://lwl.ehwqpu.com

JS:   structuredClone(obj)
来源：http://xia.sxryk.cn

TS:   structuredClone(obj)
来源：http://hqy.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://phs.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qzo.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tcu.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qgs.ybcxt.top

[K06] 解析 URL 查询串
来源：http://jgw.fengsongda.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iys.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lwu.nwbrower.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://waa.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gve.shzxlz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ffb.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hjv.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ndc.chenzaomai.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xao.sufxvd.cn

[K07] 进制转换
来源：http://nwq.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ovg.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qku.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pxx.feifeiyinyue.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://myq.nanxinkj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://umu.gotoacloud.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gyu.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jdj.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pbo.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://ibz.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://ipe.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://vvq.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://wjo.cashguo.top

TS:   v8.serialize(obj)        // Node
来源：http://edw.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ifo.gzhubu.top

Go:   encoding/gob
来源：http://rcj.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://fgc.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pzi.guowangkeji.top

================================================================================
来源：http://tmj.chenjidiqi.icu

L. 网络请求
来源：http://bdl.52xcode.cn

================================================================================
来源：http://apn.cucudq.cn

[L01] 发送 GET 请求
来源：http://txj.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tzx.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uki.haohaochexian.top

JS:   await fetch(url)
来源：http://hpe.wangdashe.top

TS:   await fetch(url)
来源：http://frf.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xhw.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://kag.fktsv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ova.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zis.feifeiyinyue.top

[L02] 发送 POST JSON
来源：http://mmd.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://cfu.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://npu.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oja.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hdf.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wdk.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dry.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bqr.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rhf.yuxming.cn

[L03] 设置自定义请求头
来源：http://bia.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aml.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fzw.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://niu.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://swy.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xkj.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lfh.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fdj.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cvs.jinyuanbaomall.cn

[L04] 设置超时
来源：http://ayu.vqdsnc.cn

Py:   requests.get(url, timeout=5)
来源：http://trb.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yhy.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uiq.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pkr.hfpthk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rfw.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wrv.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yjs.bbcook.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://umv.xziqi.cn

[L05] 上传文件（multipart）
来源：http://bnu.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ddf.cashguo.top


<!-- 参考信息 -->