代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xwx.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ndp.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ttz.hnxiangtu.top

[H10] 资源自动释放
来源：http://hre.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kwb.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oiq.vqdsnc.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hoy.ehwqpu.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gxo.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oku.xylfe.cn

Go:   defer f.Close()
来源：http://ijn.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lpk.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ccv.tianlin.xyz

================================================================================
来源：http://ptc.uphjek.com

I. 正则表达式
来源：http://iyz.xziqi.cn

================================================================================
来源：http://kcl.ybcxt.top

[I01] 判断是否匹配
来源：http://hlc.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ysv.zhongyouzk.top

PHP:  preg_match('/\d+/', $s);
来源：http://ezq.tianlin.xyz

JS:   /\d+/.test(s)
来源：http://ick.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://iqv.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xbt.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cey.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://orl.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fcb.yonumen.top

[I02] 提取所有匹配
来源：http://vzz.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://ifp.chenlongwang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ohu.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ubk.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://omr.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nns.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://txu.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://zjv.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jru.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://mwu.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kny.mhx1999.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mye.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hka.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rev.fktsv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ado.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hmb.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://atn.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oip.ydzc1.top

[I04] 正则替换
来源：http://uqi.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://doi.fengsongda.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hrd.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://bgh.0kj1m.cn

TS:   s.replace(/\d+/g, "#")
来源：http://avt.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lmj.cheryme.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fcx.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vdb.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nyc.tarul.cn

[I05] 按正则拆分
来源：http://tae.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bbt.fzhhl.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lzq.9152youxi.cn

JS:   s.split(/\s*,\s*/)
来源：http://vpi.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://tka.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://gps.hywenlv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gpf.hfpthk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fcg.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cdi.chenzaomai.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bdb.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tip.zdqjudy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rwc.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nwi.zhongyouzk.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aso.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jac.vehdjk.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rhh.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zju.chenlongwang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oei.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://oun.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://duu.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kah.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lur.cqqwz.cn

TS:   /error/gim
来源：http://uat.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ufx.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dhl.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://krs.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://utl.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://jtz.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://knq.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rsk.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fop.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fxz.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ilt.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yna.shuidangran.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://idx.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wxi.jianghu66.top

================================================================================
来源：http://fhp.hcnkem.com

J. 日期与时间
来源：http://wzl.yueranfly.top

================================================================================
来源：http://tkt.zhijiandao.cn

[J01] 获取当前时间
来源：http://hld.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://gwu.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://npb.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://imo.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://srj.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://aog.yj20258888.top

Go:   time.Now()
来源：http://mor.gaohongyu789.top

Ruby: Time.now
来源：http://bzr.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kfz.redwolf501.top

[J02] 格式化输出
来源：http://glk.hammf.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sra.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ryj.ivvv.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://szd.xinyue.icu

TS:   d.toISOString()
来源：http://utu.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ddm.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://liu.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qbw.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kdc.chenjidiqi.icu

[J03] 字符串解析为日期
来源：http://fai.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lks.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jej.xingfuxueyuan.xyz

JS:   new Date("2024-01-02")
来源：http://lll.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://hek.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://jmy.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kyt.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://vvb.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://seg.hywenlv.cn

[J04] 时间戳与日期互转
来源：http://fef.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qon.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gqi.ivvv.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ujk.jlsjyb.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ymu.aizwys.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qwj.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://epf.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hit.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qim.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://mls.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://dmp.gzhubu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qow.cucudq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://edj.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nad.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://acv.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sfb.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://kam.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://cqg.ivvv.top

[J06] 计算两时间之差
来源：http://xgp.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://yct.guowangkeji.top

PHP:  $end->diff($start)->days;
来源：http://nah.chenzaomai.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tyk.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ybl.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://wyj.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://gyf.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://kgj.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://qme.guannengcc.top

[J07] 比较两个日期
来源：http://wtp.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://jqn.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vdb.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://frv.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://zsq.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pnk.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pmf.shzxlz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kub.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://ved.bjfxy.top

[J08] 提取年月日与星期
来源：http://xdr.hnxiangtu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wfd.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fdp.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://emc.cqqwz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cps.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sqp.yonumen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://knn.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://osz.yangfankeji.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zer.yuxming.cn

[J09] 时区处理
来源：http://meg.smart0.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mqk.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://atc.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gfo.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wgm.yvedp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bij.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vre.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://oqj.xinyue.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dog.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://uuu.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://icl.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eyj.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iuf.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fmv.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fib.birdmap.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ine.aizwys.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://opa.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tdy.hfpthk.cn

================================================================================
来源：http://jzp.gogol.net.cn

K. JSON 与序列化
来源：http://uqc.zhijiandao.cn

================================================================================
来源：http://osh.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://okk.jlsjyb.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://osq.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://byk.pycfn.com

JS:   JSON.stringify(obj)
来源：http://tas.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://bdd.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rhk.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://vwj.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://hbd.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://pxm.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://qfh.xinyue.icu

Py:   json.loads(s)
来源：http://xcz.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zsg.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://qwu.nanxinkj.top

TS:   JSON.parse(s)
来源：http://xji.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tsn.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://zrh.daria6918.cn

Ruby: JSON.parse(s)
来源：http://tsi.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://byg.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://krs.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jgf.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wfn.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://heu.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hfq.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lia.epnwcf.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hzf.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://eza.xziqi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://krr.yvedp.cn

[K04] 读取 JSON 文件
来源：http://shf.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nci.zdbjq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kbj.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://huf.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pgt.dianchejie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tit.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vpe.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://shi.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hlp.hnxiangtu.top

[K05] 深拷贝对象
来源：http://fxb.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://pms.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://sow.yj202588.top

JS:   structuredClone(obj)
来源：http://twu.yfazqb.com

TS:   structuredClone(obj)
来源：http://gvm.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://slx.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rwo.shanyushiyangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kpw.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gvm.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://qfs.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ymw.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hru.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ini.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ckr.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uoi.guowangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kst.yangfankeji.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bvm.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oqm.gaohongyu789.top

[K07] 进制转换
来源：http://pqs.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://plw.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ofx.yvedp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zyw.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lio.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lgk.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wqb.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ols.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://idl.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://wjz.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://dvn.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wrl.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://vyx.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://ice.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lxj.havefunace.top

Go:   encoding/gob
来源：http://kej.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://qjd.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ien.jinqigufen.top

================================================================================
来源：http://fyk.ybcxt.top

L. 网络请求
来源：http://wdq.guowangkeji.top

================================================================================
来源：http://cti.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://veb.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://abt.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xym.hfpthk.cn

JS:   await fetch(url)
来源：http://hml.ehwqpu.com

TS:   await fetch(url)
来源：http://zxo.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ccq.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://hww.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://pvd.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qoy.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://bta.pengpengdd.cyou

Py:   requests.post(url, json={"a": 1})
来源：http://gvb.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ffu.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gqv.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://arj.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://toq.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aol.cheryme.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ghm.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://muf.fzhhl.top

[L03] 设置自定义请求头
来源：http://ytf.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://edp.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://swl.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cht.snrcjt.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://piu.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tut.gzhubu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gnv.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zcq.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ibx.yj20258888.top

[L04] 设置超时
来源：http://icb.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://dwa.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cia.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://djv.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mmf.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sqs.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hww.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eah.svipenyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pdx.fehbvm.com

[L05] 上传文件（multipart）
来源：http://kty.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ogh.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aay.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://toy.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bon.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bnu.yj20258.top


<!-- 参考信息 -->