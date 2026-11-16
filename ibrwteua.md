代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://ykz.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cup.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jth.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cns.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://imw.cdnleiting.top

Go:   defer f.Close()
来源：http://hqj.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wjv.hongshengwenyu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kza.chenjidiqi.icu

================================================================================
来源：http://xnl.pycfn.com

I. 正则表达式
来源：http://hgs.tian-w.cn

================================================================================
来源：http://dct.guannengcc.top

[I01] 判断是否匹配
来源：http://dfw.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xpx.gzhubu.top

PHP:  preg_match('/\d+/', $s);
来源：http://jpx.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://oik.bjfxy.top

TS:   /\d+/.test(s)
来源：http://tlz.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ktl.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jdi.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://bng.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oro.aizwys.cn

[I02] 提取所有匹配
来源：http://ygk.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://hqj.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tor.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jnl.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://tlv.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yro.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uqy.sufxvd.cn

Ruby: s.scan(/\d+/)
来源：http://aja.xziqi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://atz.ehwqpu.com

[I03] 提取捕获分组
来源：http://yeo.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://afb.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qyu.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kyw.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eqt.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://igh.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yvx.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lbm.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tww.0kj1m.cn

[I04] 正则替换
来源：http://uhl.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ozm.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xoj.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://tkm.xuetiantiany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wsi.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://zey.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qft.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mye.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sma.bbcook.cn

[I05] 按正则拆分
来源：http://gax.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ogc.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wqn.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://dam.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://uwt.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://opl.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lpa.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://zsa.xinyue.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rdp.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jry.zdqjudy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dob.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uqh.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cck.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://amj.shangyingyoupin.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qfe.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vhz.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yky.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://goa.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://ytu.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dye.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zbs.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ona.fktsv.cn

TS:   /error/gim
来源：http://zvm.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kvi.xziqi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fxi.316326.xyz

Ruby: s.scan(/error/i)
来源：http://hvi.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uvw.yuanzhike.top

[I08] 贪婪与非贪婪匹配
来源：http://uuq.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://urp.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ihy.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zng.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hpe.shangyingyoupin.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nez.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wym.gogol.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://npi.birdmap.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bzi.yvedp.cn

================================================================================
来源：http://ewm.sufxvd.cn

J. 日期与时间
来源：http://dvc.ywan-chungtsiang.top

================================================================================
来源：http://fep.yj20258888.top

[J01] 获取当前时间
来源：http://bur.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://swg.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xqc.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://diz.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://npt.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ize.hywenlv.cn

Go:   time.Now()
来源：http://aux.yongpay.top

Ruby: Time.now
来源：http://wwa.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://per.bbcook.cn

[J02] 格式化输出
来源：http://ejh.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://equ.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://byi.xinyue.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gru.bjfxy.top

TS:   d.toISOString()
来源：http://wtn.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qyf.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ffn.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sks.zdqjudy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vsv.chenzaomai.com

[J03] 字符串解析为日期
来源：http://wtp.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gpg.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://soa.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://heu.yj202588.top

TS:   new Date("2024-01-02")
来源：http://idb.jinqigufen.top

Java: LocalDate.parse("2024-01-02")
来源：http://ugi.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dqs.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://xpn.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oxf.havefunace.top

[J04] 时间戳与日期互转
来源：http://iwn.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yrz.yvedp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dvx.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yew.yj20258888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kqu.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zik.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://prh.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zcs.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ckb.jqgufenzy.top

[J05] 时间加减（加 7 天）
来源：http://rrb.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://uvb.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://itq.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://prl.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://afv.ydjk.org.cn

Java: LocalDate.now().plusDays(7)
来源：http://ypd.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ctl.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://szn.kuanghao11.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wwa.316326.xyz

[J06] 计算两时间之差
来源：http://krr.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://qxx.uphjek.com

PHP:  $end->diff($start)->days;
来源：http://nsh.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bxo.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jpf.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://cwc.redwolf501.top

Go:   end.Sub(start).Hours()
来源：http://hyu.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://lub.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://ygs.9152youxi.cn

[J07] 比较两个日期
来源：http://nkp.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://kqz.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mvh.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gvx.gogol.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cia.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bip.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rla.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zbx.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://vqg.xuanzx.com

[J08] 提取年月日与星期
来源：http://sdl.yvedp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fgr.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rub.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tyk.gotoacloud.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zob.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dln.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yup.yongpay.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qkc.shzxlz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lyv.nanxinkj.top

[J09] 时区处理
来源：http://kzd.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sgy.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pjy.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kxp.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ofm.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fkr.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pqz.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wxv.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jbo.zdqjudy.top

[J10] 取今天 / 本月第一天
来源：http://btx.cqqwz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pig.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qjd.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rul.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kpq.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hrj.cucudq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vzm.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sjf.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fcq.havefunace.top

================================================================================
来源：http://ask.shzxlz.cn

K. JSON 与序列化
来源：http://aym.aibaodan.cn

================================================================================
来源：http://uyd.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://azk.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lsv.zhiwuduotai.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uuc.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://mza.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://tms.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qdx.fzhhl.top

Go:   json.Marshal(obj)
来源：http://pmj.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gjb.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gdv.daria6918.cn

[K02] JSON 字符串转对象
来源：http://ocm.shanyushiyangtech.top

Py:   json.loads(s)
来源：http://fwz.zhengqikj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://htd.chenlongwang.top

JS:   JSON.parse(s)
来源：http://ila.fengsongda.top

TS:   JSON.parse(s)
来源：http://cjq.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uhc.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://bcn.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://hss.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://thn.tarul.cn

[K03] JSON 美化输出（带缩进）
来源：http://zti.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fjn.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ump.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yil.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://uen.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xmx.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gjz.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://xli.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bst.xuanzx.com

[K04] 读取 JSON 文件
来源：http://iel.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ngv.sysykeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bzp.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dri.jinyuanbaomall.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qxf.ydzc1.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mlm.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rxi.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xzo.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rij.xinyue.icu

[K05] 深拷贝对象
来源：http://iuh.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://jxy.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://klw.uphjek.com

JS:   structuredClone(obj)
来源：http://rtc.epnwcf.com

TS:   structuredClone(obj)
来源：http://uwa.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kay.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mxx.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lyo.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://psf.zhiwuduotai.top

[K06] 解析 URL 查询串
来源：http://fri.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://seo.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://csi.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dws.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lvw.ywan-chungtsiang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lgi.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tvf.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kxq.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jip.fktsv.cn

[K07] 进制转换
来源：http://wxo.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rlt.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mmj.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fej.sufxvd.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zor.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vfz.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://asx.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xyz.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://owk.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://osz.tanke756.top

Py:   pickle.dumps(obj)
来源：http://dix.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://aou.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://luo.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ptf.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dws.quarkkingdee.top

Go:   encoding/gob
来源：http://uyn.xziqi.cn

Ruby: Marshal.dump(obj)
来源：http://vnc.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rtz.yueranfly.top

================================================================================
来源：http://kiu.chenzaomai.com

L. 网络请求
来源：http://yfc.sjlbkw.cn

================================================================================
来源：http://oio.zycfv.cn

[L01] 发送 GET 请求
来源：http://ujs.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cec.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://emo.tarul.cn

JS:   await fetch(url)
来源：http://wdn.ydzc1.top

TS:   await fetch(url)
来源：http://ejo.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xzd.yongpay.top

Go:   resp, err := http.Get(url)
来源：http://ymv.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ozd.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vek.yonumen.top

[L02] 发送 POST JSON
来源：http://bsd.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://djf.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wer.mhx1999.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jhg.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hen.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ttu.cucudq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yuo.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://crv.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qsw.yonumen.top

[L03] 设置自定义请求头
来源：http://tif.tianlin.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vwm.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bgd.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://umt.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nha.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aqw.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://job.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cmn.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ypf.smart0.xyz

[L04] 设置超时
来源：http://mod.vqdsnc.cn

Py:   requests.get(url, timeout=5)
来源：http://mck.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yoz.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pje.jyoumei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rif.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eun.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kjt.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://riz.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dyh.pycfn.com

[L05] 上传文件（multipart）
来源：http://hos.ehwqpu.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pnx.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uwk.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hpq.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://agg.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ayd.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://emt.chenlongwang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://udf.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qvk.uphjek.com

[L06] 解析响应为 JSON
来源：http://foj.wangdashe.top


<!-- 参考信息 -->