代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xbs.pengpengdd.cyou

Go:   defer f.Close()
来源：http://zmh.nanxuanxn.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tgq.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ywm.smart0.xyz

================================================================================
来源：http://sbl.shanyushiyangkeji.top

I. 正则表达式
来源：http://uxm.birdmap.top

================================================================================
来源：http://glt.9152youxi.cn

[I01] 判断是否匹配
来源：http://fmp.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rww.chenlongwang.top

PHP:  preg_match('/\d+/', $s);
来源：http://vsf.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://tfo.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://mbg.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zkp.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wjx.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://glk.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ule.sufxvd.cn

[I02] 提取所有匹配
来源：http://llg.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://jko.zhiwuduotai.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sah.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fpm.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://qtf.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ebh.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://btd.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://myb.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qsd.sysykeji.top

[I03] 提取捕获分组
来源：http://caa.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://frl.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blf.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tym.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aqv.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hrd.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://swv.zhengqikj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hqj.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nqr.fengsongda.top

[I04] 正则替换
来源：http://leu.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pbq.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nia.meibo888.top

JS:   s.replace(/\d+/g, "#")
来源：http://lmo.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sex.daxiang520.top

Java: s.replaceAll("\\d+", "#")
来源：http://mik.pycfn.com

Go:   re.ReplaceAllString(s, "#")
来源：http://qul.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dhl.0kj1m.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qbl.smart0.xyz

[I05] 按正则拆分
来源：http://hpc.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vby.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xyo.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://mro.jqgfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://fjr.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://awv.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ffn.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://ssu.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pvu.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lij.sxryk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kdm.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vku.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rhs.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yyu.ydzc1.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://acr.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xxw.jinqigufen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nnk.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hlr.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://how.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ogg.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://obh.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xep.yueranfly.top

TS:   /error/gim
来源：http://wly.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qwt.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gkf.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://yyl.gogol.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ove.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://uct.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ybe.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sep.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yaf.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://coe.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hyk.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yzz.yj202588.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rax.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fpo.yj202588.top

================================================================================
来源：http://kum.chenlongwang.top

J. 日期与时间
来源：http://gmv.jinqigufen.top

================================================================================
来源：http://ici.jyoumei.cn

[J01] 获取当前时间
来源：http://xnd.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uqg.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dev.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://zfb.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://fjn.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vep.hongshengwenyu.top

Go:   time.Now()
来源：http://sdf.shuidangran.top

Ruby: Time.now
来源：http://yqq.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qtm.hesvh.cn

[J02] 格式化输出
来源：http://bfz.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qiq.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hcf.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ain.andypj.xyz

TS:   d.toISOString()
来源：http://cxw.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nox.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ycs.hesvh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fqz.jqgufenzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cnp.316326.xyz

[J03] 字符串解析为日期
来源：http://ulh.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tog.jinqigfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jsq.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://hxj.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://lbe.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fex.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lcb.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://yvz.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://osc.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://lvx.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://not.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ple.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xzb.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://faj.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mjb.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://svf.pycfn.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://brj.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dpq.andypj.xyz

[J05] 时间加减（加 7 天）
来源：http://iav.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://onf.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://nds.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cgs.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gzp.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://edy.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uks.zhijiandao.cn

Ruby: Time.now + 7 * 86400
来源：http://tnb.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://ppa.yvedp.cn

[J06] 计算两时间之差
来源：http://wdj.ybcxt.top

Py:   (end - start).total_seconds()
来源：http://xez.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://vbr.hongshengwenyu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iyh.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jsb.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gwj.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://hvo.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://cfq.meibo888.top

C#:   (end - start).TotalSeconds
来源：http://hrf.xingfuxueyuan.xyz

[J07] 比较两个日期
来源：http://jnz.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://lfm.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pak.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://uzx.vehdjk.com

TS:   d1.getTime() < d2.getTime()
来源：http://uoj.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gkc.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jhv.bbcook.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dat.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://pqv.yongpay.top

[J08] 提取年月日与星期
来源：http://qrc.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://izp.ydjk.org.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mgm.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dpl.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://exb.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kde.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://esq.jqgfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://haa.0kj1m.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hqc.kuanghao11.cn

[J09] 时区处理
来源：http://eix.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://myr.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://axn.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hdt.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jvy.ctjpmb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://llm.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wdb.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ggl.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dwz.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://jbs.fanxiaobao.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://fwu.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sug.hfpthk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ghe.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dtb.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://czg.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nrm.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ija.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qnp.c1oappe.top

================================================================================
来源：http://rtg.jlsjyb.cn

K. JSON 与序列化
来源：http://aqw.shanyushiyangtech.top

================================================================================
来源：http://dcq.yanxiufei.cn

[K01] 对象转 JSON 字符串
来源：http://tza.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xfb.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yrs.uphjek.com

JS:   JSON.stringify(obj)
来源：http://sje.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://fhb.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hrz.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://kbx.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://obu.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rqp.guannengcc.top

[K02] JSON 字符串转对象
来源：http://jgp.cqqwz.cn

Py:   json.loads(s)
来源：http://qci.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ebw.52xcode.cn

JS:   JSON.parse(s)
来源：http://xwc.daria6918.cn

TS:   JSON.parse(s)
来源：http://mzv.xuanzx.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yid.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://buv.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://lgn.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ipd.dashuyun.cn

[K03] JSON 美化输出（带缩进）
来源：http://owe.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blu.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://quw.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://qym.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qul.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aes.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ice.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bst.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gry.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://fhl.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lrl.yanxiufei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qzg.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oby.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lai.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ziz.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kjy.sweek.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ann.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tsc.tanke756.top

[K05] 深拷贝对象
来源：http://yds.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://knd.cucudq.cn

PHP:  unserialize(serialize($obj));
来源：http://nic.9152youxi.cn

JS:   structuredClone(obj)
来源：http://alw.tarul.cn

TS:   structuredClone(obj)
来源：http://phq.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jpv.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vbb.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://adx.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qtr.fengsongda.top

[K06] 解析 URL 查询串
来源：http://qtc.9152youxi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nfh.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://akz.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bva.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://enb.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uoa.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://aht.sjlbkw.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lgo.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zyc.ybcxt.top

[K07] 进制转换
来源：http://gyc.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uai.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ozs.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ipt.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cag.jinqigufen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jwc.daria6918.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nxl.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lht.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vou.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://slg.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://wvu.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://umu.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://qsg.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://faz.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://skw.epnwcf.com

Go:   encoding/gob
来源：http://srz.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://aub.fengsongda.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kug.daxiang520.top

================================================================================
来源：http://ykl.chenlongwang.top

L. 网络请求
来源：http://eqq.zhongyouzk.top

================================================================================
来源：http://fhi.bjfxy.top

[L01] 发送 GET 请求
来源：http://cwc.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://btd.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mlp.ydzc1.top

JS:   await fetch(url)
来源：http://tfc.cashguo.top

TS:   await fetch(url)
来源：http://sbh.yfazqb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xsa.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://qpk.hfpthk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://efd.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oyf.yvedp.cn

[L02] 发送 POST JSON
来源：http://ggj.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://vpb.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nst.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://roy.smart0.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jqj.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jll.tanke756.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zbt.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ndw.gotoacloud.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vid.guannengcc.top

[L03] 设置自定义请求头
来源：http://nwf.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yzg.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qof.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gxt.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://siy.yongpay.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lyz.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iax.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ete.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hhk.hfpthk.cn

[L04] 设置超时
来源：http://ain.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://fsw.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oda.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gck.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gdt.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://umf.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ssd.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ghi.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ykm.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://jea.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kvr.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ais.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rar.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://okl.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gej.jinqigufen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ena.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wko.zhoulong.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rfk.quarkkingdee.top

[L06] 解析响应为 JSON
来源：http://gxc.daria6918.cn

Py:   resp.json()
来源：http://knp.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://hej.sufxvd.cn

JS:   await resp.json()
来源：http://iun.jqgufenzy.top

TS:   await resp.json()
来源：http://hzg.shuidangran.top


<!-- 参考信息 -->