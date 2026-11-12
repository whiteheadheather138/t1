代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tzn.gogol.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jax.yj20258.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fvj.feifeiyinyue.top

[H10] 资源自动释放
来源：http://sow.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://tmn.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lkl.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wzn.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wlo.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bix.gzhubu.top

Go:   defer f.Close()
来源：http://sbf.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bec.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blv.dianchejie.cn

================================================================================
来源：http://eqp.cdnleiting.top

I. 正则表达式
来源：http://rju.zhongyouzk.top

================================================================================
来源：http://rev.aibaodan.cn

[I01] 判断是否匹配
来源：http://ylw.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mtd.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://duv.fzhhl.top

JS:   /\d+/.test(s)
来源：http://zto.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://rky.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lhp.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://umm.dianchejie.cn

Ruby: s.match?(/\d+/)
来源：http://iyt.jinqigufen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ugq.fzhhl.top

[I02] 提取所有匹配
来源：http://zcq.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://cka.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hra.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mty.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://itv.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://afn.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jsj.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://ihb.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uph.zhaomingkeji.xyz

[I03] 提取捕获分组
来源：http://wry.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ogt.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tme.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ysv.redwolf501.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://klc.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oir.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mno.shzxlz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zqs.pengpengdd.cyou

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aih.sufxvd.cn

[I04] 正则替换
来源：http://mhe.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tbo.tian-w.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://big.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ftt.yfazqb.com

TS:   s.replace(/\d+/g, "#")
来源：http://ayr.fzhhl.top

Java: s.replaceAll("\\d+", "#")
来源：http://nci.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://mzg.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tnv.yuanzhike.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cji.9152youxi.cn

[I05] 按正则拆分
来源：http://zmj.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uyr.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lwv.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://sma.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://fkz.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://czm.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://juk.yueranfly.top

Ruby: s.split(/\s*,\s*/)
来源：http://kgq.birdmap.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nbo.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hkt.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://msv.ppjwa.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xql.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vjq.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xbo.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bzw.9152youxi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yek.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zmb.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fid.yanxiufei.cn

[I07] 忽略大小写与多行模式
来源：http://dzi.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xhi.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cjm.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oqc.chenjidiqi.icu

TS:   /error/gim
来源：http://bxj.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nlc.birdmap.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://olo.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://ucf.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ggc.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://gcw.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gif.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aup.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://esx.daxiang520.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zdl.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://inu.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gxa.xuetiantiany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zxm.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ikv.svipenyu.cn

================================================================================
来源：http://jjk.birdmap.top

J. 日期与时间
来源：http://ljr.cucudq.cn

================================================================================
来源：http://tkv.yanxiufei.cn

[J01] 获取当前时间
来源：http://xse.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wit.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zsk.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://kte.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://lvm.epnwcf.com

Java: LocalDateTime.now();  Instant.now()
来源：http://skw.cashguo.top

Go:   time.Now()
来源：http://qgj.wangshuangyany.cn

Ruby: Time.now
来源：http://jju.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lkb.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://iqm.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nzv.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pkv.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nbz.0kj1m.cn

TS:   d.toISOString()
来源：http://zaa.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vop.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jeo.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://onz.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jxx.316326.xyz

[J03] 字符串解析为日期
来源：http://kle.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rey.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fhx.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://lrj.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://izk.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://pbb.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eyd.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://wqo.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wpm.tianlin.xyz

[J04] 时间戳与日期互转
来源：http://uan.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rcp.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xie.xziqi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qjz.tian-w.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ioj.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gep.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mbr.shanyushiyangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nve.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cbi.zhixingplan.top

[J05] 时间加减（加 7 天）
来源：http://yeh.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://dcy.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wof.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bkp.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uit.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://fwj.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xzt.yuxming.cn

Ruby: Time.now + 7 * 86400
来源：http://gby.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://dkk.0kj1m.cn

[J06] 计算两时间之差
来源：http://sux.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://vzm.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://flt.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vwb.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jsl.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://pto.redwolf501.top

Go:   end.Sub(start).Hours()
来源：http://hjy.cheryme.top

Ruby: end - start                 # 返回秒数
来源：http://ilc.yonumen.top

C#:   (end - start).TotalSeconds
来源：http://lvk.xingfuxueyuan.xyz

[J07] 比较两个日期
来源：http://phi.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://bky.ehwqpu.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vma.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qiu.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://rqp.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cin.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wam.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://csw.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://tfg.ydzc1.top

[J08] 提取年月日与星期
来源：http://ycs.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cxo.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fwq.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vpp.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://diu.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jrn.cashguo.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mpl.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xbk.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pwm.chenlongwang.top

[J09] 时区处理
来源：http://rtu.shuidangran.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jwh.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://asn.ivvv.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ond.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dfp.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://asi.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mlo.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://apy.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dbo.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://hbo.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vgw.fengsongda.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pfx.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qjk.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oym.sysykeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tfh.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vzf.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hlx.cucudq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ntf.vehdjk.com

================================================================================
来源：http://uju.yuxming.cn

K. JSON 与序列化
来源：http://cjt.cdnleiting.top

================================================================================
来源：http://tvz.fanxiaobao.xyz

[K01] 对象转 JSON 字符串
来源：http://ggv.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cwq.shzxlz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lel.316326.xyz

JS:   JSON.stringify(obj)
来源：http://pai.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://wlg.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wxn.yonumen.top

Go:   json.Marshal(obj)
来源：http://ndd.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lpl.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lus.pycfn.com

[K02] JSON 字符串转对象
来源：http://kin.aibaodan.cn

Py:   json.loads(s)
来源：http://sry.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rsp.yangfankeji.com

JS:   JSON.parse(s)
来源：http://ehi.cheryme.top

TS:   JSON.parse(s)
来源：http://nnn.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kpl.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://bun.cashguo.top

Ruby: JSON.parse(s)
来源：http://uat.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dbx.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://dkk.pycfn.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mgg.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rjs.iojbl.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tux.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://aba.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qwb.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fty.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://exi.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eyl.bjfxy.top

[K04] 读取 JSON 文件
来源：http://xmz.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zus.yj20258888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xkd.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pkb.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oac.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kab.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hvg.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pdn.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jqr.sxryk.cn

[K05] 深拷贝对象
来源：http://icv.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://rdo.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://tgu.birdmap.top

JS:   structuredClone(obj)
来源：http://ypr.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://bnm.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://kxm.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fer.yvedp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rnz.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nro.sweek.top

[K06] 解析 URL 查询串
来源：http://fwq.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vyb.gaohongyu789.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://whl.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wvt.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wcl.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rov.quarkkingdee.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rmn.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dmm.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xcm.tanke756.top

[K07] 进制转换
来源：http://ufx.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cbs.chenjidiqi.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fyf.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://csb.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lza.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jjb.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cco.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bry.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qko.52xcode.cn

[K08] 二进制序列化（非 JSON）
来源：http://jxl.yongpay.top

Py:   pickle.dumps(obj)
来源：http://rkj.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sth.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://yil.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://wyl.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qgf.dianchejie.cn

Go:   encoding/gob
来源：http://bke.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://ukw.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://syo.cheryme.top

================================================================================
来源：http://jyu.xingfuxueyuan.xyz

L. 网络请求
来源：http://nkd.zhengqikj.top

================================================================================
来源：http://ebn.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://rbi.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://syf.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qnn.meibo888.top

JS:   await fetch(url)
来源：http://ial.dashuyun.cn

TS:   await fetch(url)
来源：http://eyi.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ltk.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://ahm.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://jsn.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ebs.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://scs.fanxiaobao.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://xdh.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sdi.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lwz.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://krm.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gwf.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wbg.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tfj.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://srh.gzhubu.top

[L03] 设置自定义请求头
来源：http://pun.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tcw.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nui.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ava.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qtq.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nnx.haohaochexian.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rxq.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eml.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://emz.pengpengdd.cyou

[L04] 设置超时
来源：http://hgi.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://dxy.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dej.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wqh.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wjl.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vpk.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zph.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://trn.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rme.tianlin.xyz

[L05] 上传文件（multipart）
来源：http://xye.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zsl.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ogz.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yrb.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://syn.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jlj.hysaishi.cn


<!-- 参考信息 -->