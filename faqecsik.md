代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://qzx.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uxy.jinyuanbaomall.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ovj.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ifz.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mzm.chenjidiqi.icu

Go:   defer f.Close()
来源：http://nlm.yj20258888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://roe.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jmp.aizwys.cn

================================================================================
来源：http://bif.zdqjudy.top

I. 正则表达式
来源：http://ayd.9152youxi.cn

================================================================================
来源：http://jwa.ywan-chungtsiang.top

[I01] 判断是否匹配
来源：http://xcj.cucudq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sqs.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://myy.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://dms.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://sen.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ags.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hhq.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://ndb.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fkr.havefunace.top

[I02] 提取所有匹配
来源：http://rft.shzxlz.cn

Py:   re.findall(r"\d+", s)
来源：http://gnv.gotoacloud.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vfp.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mqh.tarul.cn

TS:   s.match(/\d+/g)
来源：http://suw.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lix.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://udv.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://ipk.xuetiantiany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://glh.zdbjq.cn

[I03] 提取捕获分组
来源：http://sse.hcnkem.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ekw.mhx1999.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kwp.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ssa.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zxs.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aml.smart0.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://veu.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lpk.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tao.jqgfzy.top

[I04] 正则替换
来源：http://gao.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://keu.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uec.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://qpr.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://htt.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://koh.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://udn.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ibv.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://drf.jianghu66.top

[I05] 按正则拆分
来源：http://pqm.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gnf.zhongyouzk.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://equ.c1oappe.top

JS:   s.split(/\s*,\s*/)
来源：http://gqt.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://bot.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://dbo.jiagoushi.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bpt.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://akp.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://czo.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xce.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yzd.yfazqb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dvz.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mho.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ncg.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qlo.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://agc.wangshuangyany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zjd.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pjm.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://vln.bbcook.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://amb.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vyy.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zsk.cdnleiting.top

TS:   /error/gim
来源：http://fta.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://asf.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yrf.dianchejie.cn

Ruby: s.scan(/error/i)
来源：http://row.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ltn.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://reb.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qfu.gzhubu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jrg.nanxinkj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xlu.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mgs.daxiang520.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gxm.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dkd.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ldw.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lwu.jiagoushi.top

================================================================================
来源：http://bpx.yuanzhike.top

J. 日期与时间
来源：http://naq.yuxming.cn

================================================================================
来源：http://vve.ivvv.top

[J01] 获取当前时间
来源：http://sji.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hgs.uphjek.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gkp.shuidangran.top

JS:   new Date();  Date.now()
来源：http://dys.epnwcf.com

TS:   new Date();  Date.now()
来源：http://kre.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pys.yj202588.top

Go:   time.Now()
来源：http://siv.shanyushiyangtech.top

Ruby: Time.now
来源：http://rbb.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gzs.ivvv.top

[J02] 格式化输出
来源：http://avf.feifeiyinyue.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fzs.zhixingplan.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ucl.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://roj.daxiang520.top

TS:   d.toISOString()
来源：http://odc.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://roj.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qzb.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pju.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sgx.zhengqikj.top

[J03] 字符串解析为日期
来源：http://zvn.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qxr.tianlin.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yff.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://gfb.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://ouw.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://dkf.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ngj.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://wlf.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xpu.redwolf501.top

[J04] 时间戳与日期互转
来源：http://ynd.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jqc.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tzb.yuanzhike.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xfk.guowangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pjg.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uqv.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jbf.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mad.52xcode.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vzp.cdnleiting.top

[J05] 时间加减（加 7 天）
来源：http://vut.cashguo.top

Py:   now + timedelta(days=7)
来源：http://emy.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wfd.mhx1999.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qoj.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tzw.quarkkingdee.top

Java: LocalDate.now().plusDays(7)
来源：http://feq.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wsx.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://svo.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://bwj.jiagoushi.top

[J06] 计算两时间之差
来源：http://jap.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://ovf.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://zxl.mhx1999.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yuq.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://elx.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://pam.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://mmp.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://jvs.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://rhu.shzxlz.cn

[J07] 比较两个日期
来源：http://bji.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://lmt.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hky.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://lgb.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://pri.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jsh.vqdsnc.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cfw.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eoh.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://dmj.zdqjudy.top

[J08] 提取年月日与星期
来源：http://whn.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pei.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qbt.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mph.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://haq.guowangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nfr.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ljm.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cfe.tanke756.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ffl.yongpay.top

[J09] 时区处理
来源：http://gbd.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ndm.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://elr.kuanghao11.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nlu.iojbl.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hst.guowangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nwl.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://emc.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mmd.birdmap.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mmq.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://ady.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fdj.fzhhl.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qly.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kcd.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uhr.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qho.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rmr.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yuk.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lkz.epnwcf.com

================================================================================
来源：http://aux.birdmap.top

K. JSON 与序列化
来源：http://rkb.shuidangran.top

================================================================================
来源：http://new.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://det.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qht.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xbc.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://jnk.sweek.top

TS:   JSON.stringify(obj)
来源：http://pir.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pcx.ydzc1.top

Go:   json.Marshal(obj)
来源：http://iyj.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jqh.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://yca.hywenlv.cn

[K02] JSON 字符串转对象
来源：http://lsk.cashguo.top

Py:   json.loads(s)
来源：http://kkl.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zfb.hnqzz.top

JS:   JSON.parse(s)
来源：http://ftz.cdnleiting.top

TS:   JSON.parse(s)
来源：http://can.guannengcc.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tcy.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://khn.sjlbkw.cn

Ruby: JSON.parse(s)
来源：http://hnp.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oqk.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://xip.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://opx.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oeg.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cpt.chenzaomai.com

TS:   JSON.stringify(obj, null, 2)
来源：http://eky.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nhc.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ffm.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://jhe.nanxinkj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gxl.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://uoa.svipenyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ayz.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zjg.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qat.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://avy.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nlz.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uhb.yonumen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://loo.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lim.birdmap.top

[K05] 深拷贝对象
来源：http://mhz.shuidangran.top

Py:   copy.deepcopy(obj)
来源：http://ugi.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://wmr.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://hhl.sweek.top

TS:   structuredClone(obj)
来源：http://htu.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ygv.zhijiandao.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vde.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pro.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://whd.zycfv.cn

[K06] 解析 URL 查询串
来源：http://lpv.yj20258.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vew.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://okw.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://grx.sjlbkw.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tyh.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lvp.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sxc.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ygv.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://soj.hywenlv.cn

[K07] 进制转换
来源：http://gja.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://abj.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://klw.ybcxt.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://glq.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lfb.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zwb.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nkw.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zpw.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ecv.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://nbv.sweek.top

Py:   pickle.dumps(obj)
来源：http://eou.yuanzhike.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mby.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://btb.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://qim.fanxiaobao.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mpf.sjlbkw.cn

Go:   encoding/gob
来源：http://ogc.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://roq.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iqz.9152youxi.cn

================================================================================
来源：http://ecd.gzhubu.top

L. 网络请求
来源：http://ogt.aizwys.cn

================================================================================
来源：http://moq.cucudq.cn

[L01] 发送 GET 请求
来源：http://yqu.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kjh.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iot.gotoacloud.top

JS:   await fetch(url)
来源：http://bwl.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://ncz.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nbc.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://bhn.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://icn.aizwys.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aaz.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://fnv.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://qwr.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bxx.hesvh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pag.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hal.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nxw.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dpq.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iln.wangshuangyany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cen.52xcode.cn

[L03] 设置自定义请求头
来源：http://wsn.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hir.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oic.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ptf.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dyo.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lrb.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://era.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://agy.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://typ.zhongyouzk.top

[L04] 设置超时
来源：http://nwp.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://yow.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hak.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://chx.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rsf.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rdn.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lmh.hnxiangtu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://euj.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://thd.shuidangran.top

[L05] 上传文件（multipart）
来源：http://wlq.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://arj.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gxl.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ldq.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wpe.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cut.wangshuangyany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://boq.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jtd.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bqr.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://qtm.quarkkingdee.top


<!-- 参考信息 -->