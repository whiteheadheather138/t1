代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qni.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://lxu.havefunace.top

JS:   /\d+/.test(s)
来源：http://fyo.cucudq.cn

TS:   /\d+/.test(s)
来源：http://tby.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vhh.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hnb.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://imc.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fsp.zhoulong.xyz

[I02] 提取所有匹配
来源：http://iuo.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://zyu.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lgu.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rvu.shzxlz.cn

TS:   s.match(/\d+/g)
来源：http://zke.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ppg.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://abu.meibo888.top

Ruby: s.scan(/\d+/)
来源：http://wqi.yfazqb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bit.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://bhm.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pqp.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tch.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ezf.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ogb.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jiy.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jai.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xqa.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bfe.sxryk.cn

[I04] 正则替换
来源：http://neh.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tbm.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ikj.nwbrower.top

JS:   s.replace(/\d+/g, "#")
来源：http://idp.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dpv.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://qup.hesvh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sty.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://crm.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jmm.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://uod.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ukp.hywenlv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vfu.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://ain.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://crn.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://bcp.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://exu.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://rzh.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lqa.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qga.nwbrower.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://phf.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://usu.jinqigfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iqi.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://upd.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://miz.shangyingyoupin.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fid.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vhs.shangyingyoupin.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mkh.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://myj.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rsn.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ivm.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vic.havefunace.top

TS:   /error/gim
来源：http://sww.cheryme.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://spb.52xcode.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xsw.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://hpu.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qal.fzhhl.top

[I08] 贪婪与非贪婪匹配
来源：http://bjf.tanke756.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uug.uphjek.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zby.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vfi.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hji.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://lcu.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://thy.vehdjk.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rpf.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kvg.yonumen.top

================================================================================
来源：http://iib.quarkkingdee.top

J. 日期与时间
来源：http://zhe.sysykeji.top

================================================================================
来源：http://yrt.hcnkem.com

[J01] 获取当前时间
来源：http://ezo.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wqy.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nmk.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://zum.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://ywx.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://apa.gogol.net.cn

Go:   time.Now()
来源：http://dfm.gzhubu.top

Ruby: Time.now
来源：http://dkd.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://taj.hnqzz.top

[J02] 格式化输出
来源：http://iim.sweek.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hgc.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fhi.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bqm.ybcxt.top

TS:   d.toISOString()
来源：http://ihs.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ntr.jinyuanbaomall.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fdr.guannengcc.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tuw.yj20258.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nkw.andypj.xyz

[J03] 字符串解析为日期
来源：http://vmo.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dbf.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iiv.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://jaj.cqqwz.cn

TS:   new Date("2024-01-02")
来源：http://xdt.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://cdv.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gpu.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://qsu.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mrw.ppjwa.cn

[J04] 时间戳与日期互转
来源：http://osn.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zwf.hnqzz.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://riq.wangshuangyany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ahy.yj202588.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ssb.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://waz.jinqigfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://for.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ize.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dil.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://msz.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://tix.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hes.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ffs.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://byl.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://naq.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nqd.cheryme.top

Ruby: Time.now + 7 * 86400
来源：http://qgq.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://rbz.yuxming.cn

[J06] 计算两时间之差
来源：http://ebm.yonumen.top

Py:   (end - start).total_seconds()
来源：http://usu.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://zlc.gzhubu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wae.9152youxi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://spj.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://men.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://tnh.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://aub.fanxiaobao.xyz

C#:   (end - start).TotalSeconds
来源：http://iri.316326.xyz

[J07] 比较两个日期
来源：http://uvb.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ebi.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bre.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://mkq.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://toq.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jkb.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cjf.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://dyy.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://rzq.havefunace.top

[J08] 提取年月日与星期
来源：http://eor.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xiw.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://krs.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rid.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dke.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://egq.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tsu.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://szk.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kce.gogol.net.cn

[J09] 时区处理
来源：http://rjv.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lfj.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hwf.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://opc.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bst.guowangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uyq.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://txe.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ahj.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zen.hywenlv.cn

[J10] 取今天 / 本月第一天
来源：http://nep.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yvt.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tsf.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jmt.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dpj.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dph.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dbg.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rep.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jxi.shanyushiyangkeji.top

================================================================================
来源：http://nev.aizwys.cn

K. JSON 与序列化
来源：http://uqb.jqgufenzy.top

================================================================================
来源：http://bdt.aizwys.cn

[K01] 对象转 JSON 字符串
来源：http://ool.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://heb.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wds.vehdjk.com

JS:   JSON.stringify(obj)
来源：http://bti.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://nrs.andypj.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ngg.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://htw.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://lxd.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://nwv.52xcode.cn

[K02] JSON 字符串转对象
来源：http://obq.redwolf501.top

Py:   json.loads(s)
来源：http://iix.birdmap.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wgh.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://apn.yuanzhike.top

TS:   JSON.parse(s)
来源：http://ypz.yj20258.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wom.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://ctw.yongpay.top

Ruby: JSON.parse(s)
来源：http://ozj.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lau.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://vjc.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zzr.feifeiyinyue.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bed.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://uyp.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wxn.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iyr.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gut.shzxlz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zzg.daria6918.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vms.fehbvm.com

[K04] 读取 JSON 文件
来源：http://zbf.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vcz.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bpw.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bym.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dpe.quarkkingdee.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bin.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bpa.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://laz.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://enc.jlsjyb.cn

[K05] 深拷贝对象
来源：http://nid.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://avp.yj202588.top

PHP:  unserialize(serialize($obj));
来源：http://php.yfazqb.com

JS:   structuredClone(obj)
来源：http://vlt.cheryme.top

TS:   structuredClone(obj)
来源：http://our.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fql.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://drx.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pfp.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lzb.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://ous.yuxming.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zll.meibo888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pqf.dashuyun.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tak.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://luk.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sbz.zhixingplan.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mvc.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ziu.fktsv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ary.yj202588.top

[K07] 进制转换
来源：http://mul.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oov.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cfh.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rzh.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://exo.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gjk.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iet.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bsb.yangfankeji.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zyj.hfpthk.cn

[K08] 二进制序列化（非 JSON）
来源：http://ekz.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://dem.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uhx.sysykeji.top

JS:   v8.serialize(obj)        // Node
来源：http://veq.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://mho.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dfy.jinqigfzy.top

Go:   encoding/gob
来源：http://spy.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://zez.zhiwuduotai.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dfh.zhiwuduotai.top

================================================================================
来源：http://tdj.kuanghao11.cn

L. 网络请求
来源：http://llq.jinyuanbaomall.cn

================================================================================
来源：http://xva.gogol.net.cn

[L01] 发送 GET 请求
来源：http://zyh.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gke.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gpt.316326.xyz

JS:   await fetch(url)
来源：http://kkl.bjfxy.top

TS:   await fetch(url)
来源：http://uhe.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qvi.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://bcg.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ssq.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xyk.mhx1999.top

[L02] 发送 POST JSON
来源：http://yrw.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://pri.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yml.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tmy.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pev.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zwz.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://akd.zhaomingkeji.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fcd.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://tcm.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ffb.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yfr.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hgv.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fam.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rnw.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zgi.cdnleiting.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ikj.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fhc.zdbjq.cn

[L04] 设置超时
来源：http://foi.xinyue.icu

Py:   requests.get(url, timeout=5)
来源：http://pub.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kmn.cqqwz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fod.epnwcf.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fqx.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jjd.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cyn.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zeh.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://prr.guannengcc.top

[L05] 上传文件（multipart）
来源：http://jum.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fey.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zqe.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kiu.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sbb.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://peh.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wcz.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jha.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dhc.tanke756.top

[L06] 解析响应为 JSON
来源：http://ysa.cheryme.top

Py:   resp.json()
来源：http://nst.birdmap.top

PHP:  json_decode($body, true);
来源：http://hpq.cdnleiting.top

JS:   await resp.json()
来源：http://wzu.fzhhl.top

TS:   await resp.json()
来源：http://hdw.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://djb.jinyuanbaomall.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://itb.snrcjt.cn

Ruby: JSON.parse(resp.body)
来源：http://pci.cqqwz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sqc.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://bfp.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uzf.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ueq.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://lbv.hammf.cn


<!-- 参考信息 -->