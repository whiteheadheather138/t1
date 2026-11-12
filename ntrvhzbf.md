代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://pmm.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qgr.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cav.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wsv.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lbj.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dim.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://biq.yonumen.top

[H10] 资源自动释放
来源：http://cqu.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pfz.jinqigufen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ntl.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://odh.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fbx.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pgc.jianghu66.top

Go:   defer f.Close()
来源：http://bar.9152youxi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ffr.yueranfly.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xrp.chenlongwang.top

================================================================================
来源：http://pva.havefunace.top

I. 正则表达式
来源：http://wsu.yfazqb.com

================================================================================
来源：http://uiz.snrcjt.cn

[I01] 判断是否匹配
来源：http://rsr.ywan-chungtsiang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jqt.ydzc1.top

PHP:  preg_match('/\d+/', $s);
来源：http://qeu.epnwcf.com

JS:   /\d+/.test(s)
来源：http://awt.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://hpj.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iuf.fengsongda.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gge.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://qna.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ffr.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://lif.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://ten.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jat.jiagoushi.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://csc.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://tzq.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xzh.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qnp.sufxvd.cn

Ruby: s.scan(/\d+/)
来源：http://ujg.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hhj.hcnkem.com

[I03] 提取捕获分组
来源：http://pan.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xbl.zdqjudy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zkb.xziqi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ftg.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mjh.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nld.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kfs.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rol.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bpg.nanxinkj.top

[I04] 正则替换
来源：http://ycn.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ayv.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xzo.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://pzc.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://srp.xingfuxueyuan.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://uug.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://sim.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pbg.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rnr.yanxiufei.cn

[I05] 按正则拆分
来源：http://bvk.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lyv.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://frr.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://qes.chenzaomai.com

TS:   s.split(/\s*,\s*/)
来源：http://tko.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://wlf.andypj.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dkp.fengsongda.top

Ruby: s.split(/\s*,\s*/)
来源：http://osp.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://llv.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wpd.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mvm.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pom.jinqigufen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cdf.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zdg.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://llr.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wwc.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eeu.bbcook.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gvo.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://xjo.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://coc.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qko.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://flv.yongpay.top

TS:   /error/gim
来源：http://zja.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://glq.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wfr.haohaochexian.top

Ruby: s.scan(/error/i)
来源：http://ihd.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gzr.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://xvy.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ryj.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ooy.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yfq.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://frw.cqqwz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://okp.nwbrower.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xui.cashguo.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qoi.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mdl.shanyushiyangkeji.top

================================================================================
来源：http://ehc.shangyingyoupin.top

J. 日期与时间
来源：http://yip.sjlbkw.cn

================================================================================
来源：http://erq.tanke756.top

[J01] 获取当前时间
来源：http://wnn.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://sdg.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gvp.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://vyi.sxryk.cn

TS:   new Date();  Date.now()
来源：http://bqx.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fkk.hongshengwenyu.top

Go:   time.Now()
来源：http://uuc.hongshengwenyu.top

Ruby: Time.now
来源：http://yoe.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qhr.gogol.net.cn

[J02] 格式化输出
来源：http://iah.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uab.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mrn.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://daj.jlsjyb.cn

TS:   d.toISOString()
来源：http://lfu.shanyushiyangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://soj.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://opv.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://byy.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fha.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://aoi.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nfv.cqqwz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dks.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://iof.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://ykp.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://ixq.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fmg.shangyingyoupin.top

Ruby: Date.parse("2024-01-02")
来源：http://did.haohaochexian.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://czh.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://iqi.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rxj.havefunace.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rcp.vqdsnc.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jaf.jinqigfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ukf.cqqwz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xvd.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rwk.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://add.bbcook.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jet.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://rwu.epnwcf.com

Py:   now + timedelta(days=7)
来源：http://ufa.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hca.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lek.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cnv.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://hqu.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sgc.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://ovr.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://hfn.tanke756.top

[J06] 计算两时间之差
来源：http://mbe.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://dar.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://eyd.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bcb.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://snv.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ljc.sweek.top

Go:   end.Sub(start).Hours()
来源：http://wpt.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://xma.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://ubq.cucudq.cn

[J07] 比较两个日期
来源：http://xmf.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://cxj.ybcxt.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://npx.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lyu.hammf.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ycb.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yui.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wug.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://goh.dashuyun.cn

C#:   d1 < d2;  d1 == d2
来源：http://wvi.yj20258.top

[J08] 提取年月日与星期
来源：http://fvn.ppjwa.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mbn.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wfq.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://idb.ydjk.org.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://euc.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kjy.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://btc.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rpw.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://edn.dashuyun.cn

[J09] 时区处理
来源：http://klj.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://owp.dashuyun.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nfi.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jqi.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qvf.jinyuanbaomall.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ebp.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ijc.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pxu.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nuc.xziqi.cn

[J10] 取今天 / 本月第一天
来源：http://raj.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://vqv.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qpg.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vnx.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lyb.gotoacloud.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ycm.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://flz.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hdh.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zbd.cqqwz.cn

================================================================================
来源：http://odz.guowangkeji.top

K. JSON 与序列化
来源：http://qcu.tianlin.xyz

================================================================================
来源：http://fln.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://vrw.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kpd.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jqm.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://ixv.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://lva.jlsjyb.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vgq.sjlbkw.cn

Go:   json.Marshal(obj)
来源：http://ozl.yanxiufei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zcq.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sbr.bjfxy.top

[K02] JSON 字符串转对象
来源：http://ylr.xinyue.icu

Py:   json.loads(s)
来源：http://dab.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bsx.zhengqikj.top

JS:   JSON.parse(s)
来源：http://xnp.ydzc1.top

TS:   JSON.parse(s)
来源：http://qbg.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ehf.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://tgh.yueranfly.top

Ruby: JSON.parse(s)
来源：http://ubg.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cws.andypj.xyz

[K03] JSON 美化输出（带缩进）
来源：http://yeb.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qhi.yj20258888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ant.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fbt.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lcg.zhongyouzk.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rdf.xuetiantiany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://noo.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://bny.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oaj.zhixingplan.top

[K04] 读取 JSON 文件
来源：http://bue.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zkr.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://akh.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jrq.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bus.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://goy.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bjf.tianlin.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://jab.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pnu.jyoumei.cn

[K05] 深拷贝对象
来源：http://ahe.shanyushiyangtech.top

Py:   copy.deepcopy(obj)
来源：http://eri.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://bec.jinqigufen.top

JS:   structuredClone(obj)
来源：http://nex.yangfankeji.com

TS:   structuredClone(obj)
来源：http://exc.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xje.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xvw.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://izc.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qup.uphjek.com

[K06] 解析 URL 查询串
来源：http://jeg.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ecm.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lud.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vjk.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gqs.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tna.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ghz.xuetiantiany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zus.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nlv.bjfxy.top

[K07] 进制转换
来源：http://gif.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bqx.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aky.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://app.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jmm.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gkn.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ofo.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dwv.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xtm.cashguo.top

[K08] 二进制序列化（非 JSON）
来源：http://mmt.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://tzl.hesvh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ouk.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://xnv.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://tkk.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mxg.shzxlz.cn

Go:   encoding/gob
来源：http://zmo.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://txg.jinghuilouyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tfb.yanxiufei.cn

================================================================================
来源：http://nuw.kuanghao11.cn

L. 网络请求
来源：http://pcq.hnxiangtu.top

================================================================================
来源：http://ccu.9152youxi.cn

[L01] 发送 GET 请求
来源：http://dje.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bay.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qud.jinqigufen.top

JS:   await fetch(url)
来源：http://ppc.epnwcf.com

TS:   await fetch(url)
来源：http://bgi.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yhy.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://crp.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://hwt.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ble.zdqjudy.top

[L02] 发送 POST JSON
来源：http://vgm.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://npz.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mug.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hqv.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bbi.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pih.sjlbkw.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xji.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cib.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lsk.pycfn.com

[L03] 设置自定义请求头
来源：http://aph.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ols.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://spc.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mqa.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lte.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lkb.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ayf.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dcl.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kyq.smart0.xyz

[L04] 设置超时
来源：http://aya.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://ibe.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vlz.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iny.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jxc.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wew.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kcw.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://awd.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lgo.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://fdj.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cil.meibo888.top


<!-- 参考信息 -->