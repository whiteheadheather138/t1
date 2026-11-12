代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://vnt.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ort.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sce.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gzb.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ogt.xziqi.cn

Go:   defer f.Close()
来源：http://iep.smart0.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://urm.jinqigufen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://twi.yj20258.top

================================================================================
来源：http://nhi.fktsv.cn

I. 正则表达式
来源：http://efv.snrcjt.cn

================================================================================
来源：http://jvg.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://ehv.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://adx.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://wph.ybcxt.top

JS:   /\d+/.test(s)
来源：http://peb.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://leu.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wbw.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gnr.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://ejr.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hxg.aizwys.cn

[I02] 提取所有匹配
来源：http://rth.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://gbd.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tko.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nfa.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://tvm.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gdm.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cnq.andypj.xyz

Ruby: s.scan(/\d+/)
来源：http://eto.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fsm.meibo888.top

[I03] 提取捕获分组
来源：http://gfy.ctjpmb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ayo.sweek.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ddq.cashguo.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xhv.9152youxi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xkz.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sjk.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wjb.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zft.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cmh.sxryk.cn

[I04] 正则替换
来源：http://mjr.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://eyv.fanxiaobao.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kmg.jinqigfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://tni.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dei.mhx1999.top

Java: s.replaceAll("\\d+", "#")
来源：http://mhg.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yju.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hmw.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yte.fktsv.cn

[I05] 按正则拆分
来源：http://nji.yueranfly.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wup.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tjm.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://smn.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://lif.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://noi.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hwx.zdbjq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://aoq.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lcq.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ilf.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tnh.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fub.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hpe.tarul.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hwd.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rwd.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wmc.0kj1m.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fru.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oth.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://zwx.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gfx.xylfe.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cel.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://edv.dashuyun.cn

TS:   /error/gim
来源：http://rls.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://scl.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jvj.zhixingplan.top

Ruby: s.scan(/error/i)
来源：http://eao.xziqi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kxv.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://uvj.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aol.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cpc.zhijiandao.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zoi.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bvp.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://mgh.sweek.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xzr.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ctw.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://scj.gzhubu.top

================================================================================
来源：http://hpu.yuanzhike.top

J. 日期与时间
来源：http://qnf.ppjwa.cn

================================================================================
来源：http://nph.sweek.top

[J01] 获取当前时间
来源：http://vii.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hqy.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rne.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://nez.epnwcf.com

TS:   new Date();  Date.now()
来源：http://lej.chenjidiqi.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://kdo.kuanghao11.cn

Go:   time.Now()
来源：http://pgs.hfpthk.cn

Ruby: Time.now
来源：http://eam.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ucs.cucudq.cn

[J02] 格式化输出
来源：http://ggr.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rlp.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sse.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://agn.birdmap.top

TS:   d.toISOString()
来源：http://gxt.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ngq.jinyuanbaomall.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pcc.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ayo.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ekt.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://yng.zhaomingkeji.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://elb.ywan-chungtsiang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yhq.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://wyv.jinyuanbaomall.cn

TS:   new Date("2024-01-02")
来源：http://cna.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://dfh.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vyy.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://jck.yuxming.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aqu.ydzc1.top

[J04] 时间戳与日期互转
来源：http://mcj.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hjj.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wsf.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eac.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://bvc.redwolf501.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xbt.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mzw.ydjk.org.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://whp.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uuz.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://trg.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://mrs.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sfb.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gds.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gyj.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://ipi.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oob.sweek.top

Ruby: Time.now + 7 * 86400
来源：http://quj.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://rdo.fktsv.cn

[J06] 计算两时间之差
来源：http://viz.chenjidiqi.icu

Py:   (end - start).total_seconds()
来源：http://oqp.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://vrp.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://txr.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xzy.yuxming.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ott.hywenlv.cn

Go:   end.Sub(start).Hours()
来源：http://zua.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://izt.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://shu.sxryk.cn

[J07] 比较两个日期
来源：http://wgq.smart0.xyz

Py:   d1 < d2;  d1 == d2
来源：http://xre.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fxb.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://sfn.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cdb.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sty.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nnm.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://mbb.andypj.xyz

C#:   d1 < d2;  d1 == d2
来源：http://dqi.xziqi.cn

[J08] 提取年月日与星期
来源：http://pbr.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gnl.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fjp.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wsp.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://clh.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bno.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yjp.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://irp.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xta.zhixingplan.top

[J09] 时区处理
来源：http://byi.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gjq.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nds.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qzx.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wpa.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pkx.nanxinkj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nll.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://vrh.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qvs.yvedp.cn

[J10] 取今天 / 本月第一天
来源：http://avz.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dmi.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ket.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ayk.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yby.shanyushiyangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dwz.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yrd.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vwg.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://biq.jinqigufen.top

================================================================================
来源：http://yhj.sjlbkw.cn

K. JSON 与序列化
来源：http://oyf.tianlin.xyz

================================================================================
来源：http://gwi.jiagoushi.top

[K01] 对象转 JSON 字符串
来源：http://hhb.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qmk.hysaishi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://evd.yj202588.top

JS:   JSON.stringify(obj)
来源：http://cwx.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://irk.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lab.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://jkp.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://eng.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ara.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://lgr.uphjek.com

Py:   json.loads(s)
来源：http://aau.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mty.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://dmd.aizwys.cn

TS:   JSON.parse(s)
来源：http://mzr.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yjd.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://ind.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://rct.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://chq.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://ppc.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fqa.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rgy.xziqi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://afh.shangyingyoupin.top

TS:   JSON.stringify(obj, null, 2)
来源：http://udb.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://int.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://snu.ywan-chungtsiang.top

Ruby: JSON.pretty_generate(obj)
来源：http://asu.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ifq.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://vzp.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zwd.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qdk.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ovu.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rma.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lql.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ktf.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sfw.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wza.andypj.xyz

[K05] 深拷贝对象
来源：http://fqu.svipenyu.cn

Py:   copy.deepcopy(obj)
来源：http://rjq.gogol.net.cn

PHP:  unserialize(serialize($obj));
来源：http://azs.nwbrower.top

JS:   structuredClone(obj)
来源：http://pmf.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://vnt.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ibl.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pts.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lzi.aibaodan.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rts.nwbrower.top

[K06] 解析 URL 查询串
来源：http://mnu.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kli.hywenlv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iil.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hbb.sysykeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pvk.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jlw.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://igt.ybcxt.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://onq.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lxt.jqgufenzy.top

[K07] 进制转换
来源：http://rhn.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://enx.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ydh.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wpc.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uqm.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iqz.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mzd.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wrr.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iin.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://rjn.xuetiantiany.cn

Py:   pickle.dumps(obj)
来源：http://opu.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://bay.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://kyx.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://vem.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pge.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://ipu.shzxlz.cn

Ruby: Marshal.dump(obj)
来源：http://ffr.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rlq.fzhhl.top

================================================================================
来源：http://wvw.yfazqb.com

L. 网络请求
来源：http://rqi.zhengqikj.top

================================================================================
来源：http://blc.gotoacloud.top

[L01] 发送 GET 请求
来源：http://esg.zhongyouzk.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nnw.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lwn.xuetiantiany.cn

JS:   await fetch(url)
来源：http://lvf.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://swo.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lqm.ehwqpu.com

Go:   resp, err := http.Get(url)
来源：http://wvf.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://thq.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dwt.fktsv.cn

[L02] 发送 POST JSON
来源：http://zor.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://asv.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://psz.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qdt.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://unq.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tej.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rcn.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ttl.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uiu.zhengqikj.top

[L03] 设置自定义请求头
来源：http://kdf.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hqc.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aoh.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jww.iojbl.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xxu.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uwt.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zld.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hom.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lcc.xylfe.cn

[L04] 设置超时
来源：http://pqu.feifeiyinyue.top

Py:   requests.get(url, timeout=5)
来源：http://vep.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fao.gogol.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tci.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ryr.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qcz.zhiwuduotai.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://joq.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hqt.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tyu.zycfv.cn

[L05] 上传文件（multipart）
来源：http://fcv.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nml.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bvn.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kuz.hfpthk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dpp.yuxming.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tfm.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ixr.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://diy.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ipt.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://xxp.quarkkingdee.top


<!-- 参考信息 -->