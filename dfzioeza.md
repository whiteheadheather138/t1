代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zyd.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://yws.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xdw.dianchejie.cn

[H10] 资源自动释放
来源：http://ogq.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://nnu.guowangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://npr.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ifq.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ygd.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sfr.aizwys.cn

Go:   defer f.Close()
来源：http://itz.sysykeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bzw.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vbm.hongshengwenyu.top

================================================================================
来源：http://fag.gotoacloud.top

I. 正则表达式
来源：http://ccz.nanxinkj.top

================================================================================
来源：http://ith.yueranfly.top

[I01] 判断是否匹配
来源：http://eyi.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hwb.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pfd.epnwcf.com

JS:   /\d+/.test(s)
来源：http://zhh.uphjek.com

TS:   /\d+/.test(s)
来源：http://zdz.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dbc.redwolf501.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fgi.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://dzr.xylfe.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dzv.zhengqikj.top

[I02] 提取所有匹配
来源：http://whj.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://xdp.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zjg.shanyushiyangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cun.nanxuanxn.top

TS:   s.match(/\d+/g)
来源：http://qzm.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ham.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://srb.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://ffo.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xev.yvedp.cn

[I03] 提取捕获分组
来源：http://psm.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://egs.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vhp.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oaw.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xdw.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fuc.jqgufenzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://chv.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bxs.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fqg.redwolf501.top

[I04] 正则替换
来源：http://hln.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mdr.hcnkem.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uzh.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gsa.aibaodan.cn

TS:   s.replace(/\d+/g, "#")
来源：http://frf.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nxf.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://jhh.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eva.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bur.epnwcf.com

[I05] 按正则拆分
来源：http://urz.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mus.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sbz.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://evj.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://qmc.hfpthk.cn

Java: s.split("\\s*,\\s*")
来源：http://gtn.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wrn.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bim.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ojc.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nmx.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iar.jianghu66.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tox.9152youxi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fxi.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tij.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jyn.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lsy.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ggz.hnqzz.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qnc.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://ehv.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mvn.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dlm.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tns.smart0.xyz

TS:   /error/gim
来源：http://lah.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ivz.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mpz.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://tsz.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://itb.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://afr.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ohw.ppjwa.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kum.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mkq.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sbb.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://ydj.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gfk.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bmg.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aqe.fanxiaobao.xyz

================================================================================
来源：http://fty.yuxming.cn

J. 日期与时间
来源：http://xzj.yfazqb.com

================================================================================
来源：http://lpz.uphjek.com

[J01] 获取当前时间
来源：http://orf.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xfn.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hfg.yongpay.top

JS:   new Date();  Date.now()
来源：http://wbm.snrcjt.cn

TS:   new Date();  Date.now()
来源：http://lbd.ywan-chungtsiang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jok.ehwqpu.com

Go:   time.Now()
来源：http://dic.yangfankeji.com

Ruby: Time.now
来源：http://yst.svipenyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://esn.zhoulong.xyz

[J02] 格式化输出
来源：http://xyg.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mlt.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dsm.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://djv.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://pdf.birdmap.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vmt.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mlf.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eqk.smart0.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dwy.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://pck.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://brm.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zvj.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://egd.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://etc.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://kmn.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ctm.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://qng.jinqigufen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://inz.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://upi.shzxlz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://otd.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hrh.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zrv.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://eax.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://meg.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hos.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kqe.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cvk.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://ooe.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://vlu.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fjk.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tdw.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltj.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://beg.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lfg.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://vbm.kuanghao11.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rvj.shuidangran.top

[J06] 计算两时间之差
来源：http://lne.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://jht.jqgfzy.top

PHP:  $end->diff($start)->days;
来源：http://tbo.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ole.cashguo.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://spg.yuxming.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vgg.jiagoushi.top

Go:   end.Sub(start).Hours()
来源：http://ism.cdnleiting.top

Ruby: end - start                 # 返回秒数
来源：http://yys.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://eqj.jlsjyb.cn

[J07] 比较两个日期
来源：http://juu.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://trg.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://khf.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://afi.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://mrr.yangfankeji.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qlx.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tqe.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jzc.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://qxw.yfazqb.com

[J08] 提取年月日与星期
来源：http://nhg.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rvs.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qmv.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kic.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jms.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uvo.ydzc1.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lph.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ual.yj202588.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://juv.hesvh.cn

[J09] 时区处理
来源：http://igi.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mpo.vehdjk.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fbe.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tzn.hywenlv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cwn.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://djx.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cse.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ihd.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://buq.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://rjp.fanxiaobao.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://drd.hnxiangtu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ihd.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://heu.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mor.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://khu.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blk.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vgn.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fwi.hywenlv.cn

================================================================================
来源：http://ljs.birdmap.top

K. JSON 与序列化
来源：http://jyk.cqqwz.cn

================================================================================
来源：http://tfe.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://ghq.jyoumei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wiz.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nyu.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://lqa.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://ero.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uix.mhx1999.top

Go:   json.Marshal(obj)
来源：http://jjy.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xeb.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hqw.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://cms.meibo888.top

Py:   json.loads(s)
来源：http://qqs.hysaishi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://evg.yvedp.cn

JS:   JSON.parse(s)
来源：http://kfp.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://vfb.yangfankeji.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qus.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://tnw.ehwqpu.com

Ruby: JSON.parse(s)
来源：http://wzv.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://exv.jlsjyb.cn

[K03] JSON 美化输出（带缩进）
来源：http://jui.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ttj.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ylv.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://xnk.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yvx.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://biw.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blp.jyoumei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kbq.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ldx.c1oappe.top

[K04] 读取 JSON 文件
来源：http://njy.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://syg.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tsz.sxryk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pyq.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kwa.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wds.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hyg.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://cnb.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wld.hnqzz.top

[K05] 深拷贝对象
来源：http://ihd.zhoulong.xyz

Py:   copy.deepcopy(obj)
来源：http://jhx.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://lqe.jianghu66.top

JS:   structuredClone(obj)
来源：http://dtf.haohaochexian.top

TS:   structuredClone(obj)
来源：http://awn.ydzc1.top

Java: // 手写拷贝构造，或序列化往返
来源：http://onw.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bkh.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qpi.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ecy.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://dpl.shangyingyoupin.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zir.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nam.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nxv.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://osw.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qtf.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://isl.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aps.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wiz.zdbjq.cn

[K07] 进制转换
来源：http://gja.fktsv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://huj.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lno.svipenyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qmg.ybcxt.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zgk.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xmt.jinyuanbaomall.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lfn.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qbp.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qrz.zhongyouzk.top

[K08] 二进制序列化（非 JSON）
来源：http://kmu.quarkkingdee.top

Py:   pickle.dumps(obj)
来源：http://wff.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cex.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://xku.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://ybk.ppjwa.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://edj.aizwys.cn

Go:   encoding/gob
来源：http://msg.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://zgc.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wmn.yfazqb.com

================================================================================
来源：http://ped.snrcjt.cn

L. 网络请求
来源：http://nss.nwbrower.top

================================================================================
来源：http://pdo.smart0.xyz

[L01] 发送 GET 请求
来源：http://qta.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ifa.pycfn.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sgw.havefunace.top

JS:   await fetch(url)
来源：http://vyp.fzhhl.top

TS:   await fetch(url)
来源：http://scf.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gym.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://ufx.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mzb.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ydf.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://ead.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://pef.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wvq.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nyu.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ino.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xcv.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zti.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kcp.sxryk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://get.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://frc.yfazqb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zbf.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nuv.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tyy.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hnb.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lbp.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iyw.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gtn.sysykeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pfh.ydjk.org.cn

[L04] 设置超时
来源：http://mpa.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://zqn.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hmx.snrcjt.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rap.birdmap.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mhp.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rio.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wwk.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mms.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://byo.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://hcu.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wzk.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rwc.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kve.quarkkingdee.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mcs.gaohongyu789.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xrs.yangfankeji.com


<!-- 参考信息 -->