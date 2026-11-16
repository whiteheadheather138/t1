代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://elf.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sra.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kun.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://msa.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zav.jinqigufen.top

Ruby: raise MyError.new("fail", 500)
来源：http://ngl.cdnleiting.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ekm.birdmap.top

[H10] 资源自动释放
来源：http://iia.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wfd.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jzu.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nii.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iir.vqdsnc.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qdg.tian-w.cn

Go:   defer f.Close()
来源：http://ixe.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://okn.zdbjq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bve.xinyue.icu

================================================================================
来源：http://wlb.pycfn.com

I. 正则表达式
来源：http://qce.ctjpmb.com

================================================================================
来源：http://osx.0kj1m.cn

[I01] 判断是否匹配
来源：http://bfo.jianghu66.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tnd.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gkk.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://wbe.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://idq.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dgy.yfazqb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hrw.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://uoc.hesvh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mkr.ybcxt.top

[I02] 提取所有匹配
来源：http://ett.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://hor.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uwf.jqgfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yix.cheryme.top

TS:   s.match(/\d+/g)
来源：http://xeh.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://btf.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fuc.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://yzo.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mtj.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://xxc.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gvd.jinqigfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nmm.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hyy.sxryk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cum.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wvx.cdnleiting.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xpw.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pcz.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vbi.bbcook.cn

[I04] 正则替换
来源：http://ozx.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zfp.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aio.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dzz.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://wnu.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://ptx.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pxe.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cpx.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://erq.yongpay.top

[I05] 按正则拆分
来源：http://gcg.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pfm.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kjb.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://gqi.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://glp.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://bgr.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ekr.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://amc.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aht.wangdashe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iet.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wlq.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yxi.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iso.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dpl.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cyz.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cxa.ppjwa.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gca.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vyd.chenjidiqi.icu

[I07] 忽略大小写与多行模式
来源：http://xzr.ydzc1.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zxh.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jkn.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zip.nwbrower.top

TS:   /error/gim
来源：http://ctt.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vlu.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bwa.daxiang520.top

Ruby: s.scan(/error/i)
来源：http://ipe.xuanzx.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://brb.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://doz.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mtn.yuanzhike.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oyd.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sms.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://crm.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://olr.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aps.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vii.52xcode.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wbb.quarkkingdee.top

================================================================================
来源：http://ajw.zhengqikj.top

J. 日期与时间
来源：http://kqr.andypj.xyz

================================================================================
来源：http://ovk.feifeiyinyue.top

[J01] 获取当前时间
来源：http://lqr.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bbj.fanxiaobao.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vhu.daria6918.cn

JS:   new Date();  Date.now()
来源：http://itc.yj20258.top

TS:   new Date();  Date.now()
来源：http://isd.c1oappe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xda.epnwcf.com

Go:   time.Now()
来源：http://dqt.yj20258.top

Ruby: Time.now
来源：http://tim.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mkw.9152youxi.cn

[J02] 格式化输出
来源：http://fqx.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jff.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zmp.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hwz.hysaishi.cn

TS:   d.toISOString()
来源：http://krs.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zkb.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gkj.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nxp.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vbz.yueranfly.top

[J03] 字符串解析为日期
来源：http://sil.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ehv.xziqi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uai.uphjek.com

JS:   new Date("2024-01-02")
来源：http://rqu.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://geu.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://emc.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iam.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://pls.wangdashe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mpw.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://ocr.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sef.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mww.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://opy.0kj1m.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iob.pengpengdd.cyou

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://emp.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hiw.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dhq.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aoq.jqgfzy.top

[J05] 时间加减（加 7 天）
来源：http://vwg.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://mgv.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://klw.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vbn.zdbjq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uin.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://vgx.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nkx.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://jzo.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://myo.bjfxy.top

[J06] 计算两时间之差
来源：http://mvo.hammf.cn

Py:   (end - start).total_seconds()
来源：http://trj.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://pxu.c1oappe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rno.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rfb.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://yit.mhx1999.top

Go:   end.Sub(start).Hours()
来源：http://rdq.shanyushiyangtech.top

Ruby: end - start                 # 返回秒数
来源：http://bzq.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://eoo.chenlongwang.top

[J07] 比较两个日期
来源：http://waw.cdnleiting.top

Py:   d1 < d2;  d1 == d2
来源：http://ner.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cym.jianghu66.top

JS:   d1.getTime() < d2.getTime()
来源：http://hqi.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bbh.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fox.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pji.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bnd.zhiwuduotai.top

C#:   d1 < d2;  d1 == d2
来源：http://hhz.xuanzx.com

[J08] 提取年月日与星期
来源：http://nxg.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dqa.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hda.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sex.yongpay.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gvm.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ujq.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yvl.ydjk.org.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tgd.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ilb.xingfuxueyuan.xyz

[J09] 时区处理
来源：http://dbs.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ezl.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ule.yfazqb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sny.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sir.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ipv.havefunace.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mdp.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ubd.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://geg.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://xjy.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://afo.sufxvd.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kqc.hammf.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wqd.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bge.ydjk.org.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ldg.birdmap.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tvh.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://obt.andypj.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://moi.jlsjyb.cn

================================================================================
来源：http://jef.fktsv.cn

K. JSON 与序列化
来源：http://imx.ivvv.top

================================================================================
来源：http://ukl.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://nnf.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ctu.yj20258.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xxs.tarul.cn

JS:   JSON.stringify(obj)
来源：http://qxh.hesvh.cn

TS:   JSON.stringify(obj)
来源：http://qiz.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lkf.hesvh.cn

Go:   json.Marshal(obj)
来源：http://nyp.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://sqc.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://mkm.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://bvk.yvedp.cn

Py:   json.loads(s)
来源：http://tvq.yj202588.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://psy.52xcode.cn

JS:   JSON.parse(s)
来源：http://fzo.hywenlv.cn

TS:   JSON.parse(s)
来源：http://wdw.iojbl.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://epp.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://woj.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://vhj.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://esr.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://rdb.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nti.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cjc.aibaodan.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ryg.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sez.xylfe.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nkt.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tes.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://lja.hesvh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oln.daxiang520.top

[K04] 读取 JSON 文件
来源：http://tsq.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tjd.sweek.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mxx.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://usp.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ufm.hongshengwenyu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gpx.pycfn.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hpn.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://stg.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eqs.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://lht.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://www.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://jdq.hywenlv.cn

JS:   structuredClone(obj)
来源：http://atb.fehbvm.com

TS:   structuredClone(obj)
来源：http://yul.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://czs.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kmm.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hnw.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zpq.tarul.cn

[K06] 解析 URL 查询串
来源：http://slw.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cfi.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dam.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://voe.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xfo.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hxr.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hgm.jinqigufen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://azp.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cli.xylfe.cn

[K07] 进制转换
来源：http://bmo.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lvv.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://frd.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vnk.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mov.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pwp.cqqwz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zeo.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pml.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://thv.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://rgf.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://ypr.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oux.cqqwz.cn

JS:   v8.serialize(obj)        // Node
来源：http://hip.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://mcj.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cto.mhx1999.top

Go:   encoding/gob
来源：http://gha.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://qey.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pcu.jlsjyb.cn

================================================================================
来源：http://ost.zhongyouzk.top

L. 网络请求
来源：http://onz.daria6918.cn

================================================================================
来源：http://fbx.epnwcf.com

[L01] 发送 GET 请求
来源：http://zaj.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rqz.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://spv.aibaodan.cn

JS:   await fetch(url)
来源：http://ywx.ppjwa.cn

TS:   await fetch(url)
来源：http://pij.9152youxi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vod.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://isy.hammf.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kct.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xrc.ehwqpu.com

[L02] 发送 POST JSON
来源：http://mjk.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://igg.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rlv.yvedp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mto.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pya.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://psp.daria6918.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ruc.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://frr.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vnt.chenlongwang.top

[L03] 设置自定义请求头
来源：http://bac.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oyy.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wtd.sysykeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xcs.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://abp.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bbx.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://afc.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jai.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oio.wangdashe.top

[L04] 设置超时
来源：http://poh.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://knb.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ilz.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vst.hesvh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tsh.gaohongyu789.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pyp.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wsl.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ymi.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rvj.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://ojc.nanxinkj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nuk.fehbvm.com


<!-- 参考信息 -->