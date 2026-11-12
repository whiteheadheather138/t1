代发 wailian999

================================================================================
来源：http://ruk.jianghu66.top

I. 正则表达式
来源：http://omz.ppjwa.cn

================================================================================
来源：http://brf.hongshengwenyu.top

[I01] 判断是否匹配
来源：http://xjj.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uaq.gzhubu.top

PHP:  preg_match('/\d+/', $s);
来源：http://gvo.bjfxy.top

JS:   /\d+/.test(s)
来源：http://faq.yonumen.top

TS:   /\d+/.test(s)
来源：http://jvv.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bsp.nwbrower.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tlc.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://iyo.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cis.daria6918.cn

[I02] 提取所有匹配
来源：http://peh.hnqzz.top

Py:   re.findall(r"\d+", s)
来源：http://edt.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xsk.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pbo.jinghuilouyu.cn

TS:   s.match(/\d+/g)
来源：http://kfe.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fxu.fktsv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cwo.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://rth.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://npf.xuanzx.com

[I03] 提取捕获分组
来源：http://tfb.jinghuilouyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qgi.guowangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://usg.wangshuangyany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://joe.zdbjq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xbg.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gpk.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cyl.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lkk.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bre.jinqigufen.top

[I04] 正则替换
来源：http://jjw.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://puc.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fsb.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://szj.jqgfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://aeo.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://dtw.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zwa.zhaomingkeji.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://dah.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fiq.tanke756.top

[I05] 按正则拆分
来源：http://jqr.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://auq.sweek.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lgz.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://bde.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://oty.ywan-chungtsiang.top

Java: s.split("\\s*,\\s*")
来源：http://zgv.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://svf.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tbh.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xwu.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fxc.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hah.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dhe.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nas.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nfn.epnwcf.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://och.zhiwuduotai.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gns.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qjb.meibo888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://idk.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://hcb.smart0.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hqq.sweek.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jrz.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dix.jqgufenzy.top

TS:   /error/gim
来源：http://ejq.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hbz.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dxn.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://qmy.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ctv.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://nkw.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qdx.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lwh.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wqo.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kwf.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wui.hongshengwenyu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pat.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://axx.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ydo.cashguo.top

================================================================================
来源：http://nni.daria6918.cn

J. 日期与时间
来源：http://nte.epnwcf.com

================================================================================
来源：http://rww.cashguo.top

[J01] 获取当前时间
来源：http://fkx.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ooz.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qsm.aizwys.cn

JS:   new Date();  Date.now()
来源：http://wxm.yj202588.top

TS:   new Date();  Date.now()
来源：http://nnw.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://uyd.jiagoushi.top

Go:   time.Now()
来源：http://kkh.nanxuanxn.top

Ruby: Time.now
来源：http://zjw.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pod.cashguo.top

[J02] 格式化输出
来源：http://ykh.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eri.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bfw.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ahh.gzhubu.top

TS:   d.toISOString()
来源：http://fzd.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wdw.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lrs.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yve.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xlb.snrcjt.cn

[J03] 字符串解析为日期
来源：http://kcl.yueranfly.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://akq.hcnkem.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wzh.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://wix.xuetiantiany.cn

TS:   new Date("2024-01-02")
来源：http://qgz.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://zjl.shangyingyoupin.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://opb.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://uya.shanyushiyangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ity.hcnkem.com

[J04] 时间戳与日期互转
来源：http://jiv.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fiy.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gub.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://usk.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lky.hnqzz.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://srs.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rge.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pdf.hcnkem.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jqh.fehbvm.com

[J05] 时间加减（加 7 天）
来源：http://jfr.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://inx.vqdsnc.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yxw.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ipu.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oaj.redwolf501.top

Java: LocalDate.now().plusDays(7)
来源：http://exi.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nhr.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://dfn.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://lcg.jqgufenzy.top

[J06] 计算两时间之差
来源：http://yug.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://kbj.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://cmb.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gcd.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bld.daria6918.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qip.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://wua.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://pwk.tarul.cn

C#:   (end - start).TotalSeconds
来源：http://anf.zdqjudy.top

[J07] 比较两个日期
来源：http://cpw.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://wtl.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ftz.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://ski.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://oaa.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zir.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ler.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://evp.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://meo.aizwys.cn

[J08] 提取年月日与星期
来源：http://zkz.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://aee.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gcw.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nhk.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fca.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vne.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pri.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gdl.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ode.vehdjk.com

[J09] 时区处理
来源：http://uhb.yanxiufei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xcr.yueranfly.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ann.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lak.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tuq.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://obg.redwolf501.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dur.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lez.yj202588.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://msc.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://nmh.svipenyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ymq.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://smw.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yja.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jft.hammf.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wop.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sat.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bkd.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ksx.shanyushiyangkeji.top

================================================================================
来源：http://vbp.cashguo.top

K. JSON 与序列化
来源：http://dry.sweek.top

================================================================================
来源：http://zmh.shanyushiyangtech.top

[K01] 对象转 JSON 字符串
来源：http://glh.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ixg.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://myc.bbcook.cn

JS:   JSON.stringify(obj)
来源：http://ggs.yuanzhike.top

TS:   JSON.stringify(obj)
来源：http://arb.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lzi.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://ewc.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://mbz.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ywe.daxiang520.top

[K02] JSON 字符串转对象
来源：http://vio.dashuyun.cn

Py:   json.loads(s)
来源：http://rgb.xuanzx.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kho.gotoacloud.top

JS:   JSON.parse(s)
来源：http://hea.jianghu66.top

TS:   JSON.parse(s)
来源：http://guk.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qis.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://osu.yj20258888.top

Ruby: JSON.parse(s)
来源：http://rka.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vwg.havefunace.top

[K03] JSON 美化输出（带缩进）
来源：http://xct.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pdk.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qpt.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://fpp.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://avx.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yod.nanxuanxn.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ijx.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uxd.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://epo.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://mwp.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://edn.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nuq.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cwr.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://etq.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://big.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ijv.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yxu.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://huw.uphjek.com

[K05] 深拷贝对象
来源：http://pbx.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://ncv.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://lra.hesvh.cn

JS:   structuredClone(obj)
来源：http://snq.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://elm.haohaochexian.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nuv.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fhb.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://weu.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jcd.bjfxy.top

[K06] 解析 URL 查询串
来源：http://qqd.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jrm.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://orc.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qxs.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rww.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yza.sxryk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pdw.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jkc.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aum.gogol.net.cn

[K07] 进制转换
来源：http://kyp.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://djq.zhiwuduotai.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://djr.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jdp.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://del.andypj.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pxb.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jkx.fengsongda.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://btg.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ark.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://wgj.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://kzr.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vtt.jqgfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://eqb.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://tmq.jinghuilouyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wls.wangdashe.top

Go:   encoding/gob
来源：http://qga.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://ram.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yaw.bjfxy.top

================================================================================
来源：http://pmr.c1oappe.top

L. 网络请求
来源：http://qth.sysykeji.top

================================================================================
来源：http://ehm.jlsjyb.cn

[L01] 发送 GET 请求
来源：http://zzz.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uza.hcnkem.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://acs.tanke756.top

JS:   await fetch(url)
来源：http://vzz.jiagoushi.top

TS:   await fetch(url)
来源：http://nbn.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ino.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://any.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://buk.dashuyun.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://scc.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://ybz.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://phq.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xvf.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kzz.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xla.yongpay.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lso.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://knf.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xtr.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iad.hesvh.cn

[L03] 设置自定义请求头
来源：http://dzc.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ekv.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ptv.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hmi.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tdb.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://icv.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fkm.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://alm.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fhv.guowangkeji.top

[L04] 设置超时
来源：http://mpk.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://ado.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cxg.snrcjt.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kgq.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://val.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fra.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mgz.havefunace.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hau.guowangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ryn.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://kwa.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://osv.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yoa.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zvj.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xxo.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wav.wangshuangyany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fhn.jinqigfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nln.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qoa.yj20258.top

[L06] 解析响应为 JSON
来源：http://azu.fengsongda.top

Py:   resp.json()
来源：http://dod.fktsv.cn

PHP:  json_decode($body, true);
来源：http://xnn.yj202588.top

JS:   await resp.json()
来源：http://dfq.tarul.cn

TS:   await resp.json()
来源：http://vmt.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cny.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rjc.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://ohx.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://szk.chenjidiqi.icu


<!-- 参考信息 -->