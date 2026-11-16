代发 wailian999

[I02] 提取所有匹配
来源：http://gwy.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://gox.yfazqb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pad.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://joa.hywenlv.cn

TS:   s.match(/\d+/g)
来源：http://ufh.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hfb.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ysv.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://bur.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bqm.zdbjq.cn

[I03] 提取捕获分组
来源：http://tuf.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cun.chenzaomai.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bpp.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://txl.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jse.zhongyouzk.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xmo.gotoacloud.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oyu.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ber.hnxiangtu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gmo.chenjidiqi.icu

[I04] 正则替换
来源：http://jla.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://adp.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bho.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://goj.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://jpt.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://nfj.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://rsa.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xnj.nanxuanxn.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ioz.cqqwz.cn

[I05] 按正则拆分
来源：http://vli.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ped.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zqy.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://veq.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://mvp.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://ltt.pengpengdd.cyou

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zqi.xylfe.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bkj.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vub.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zkb.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ryq.iojbl.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hxw.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ekb.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aef.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zhc.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hnc.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sal.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tzy.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://skg.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ino.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://epy.jlsjyb.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bho.jyoumei.cn

TS:   /error/gim
来源：http://efv.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xoj.chenjidiqi.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hlt.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://scf.cqqwz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lzd.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://egq.tarul.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://khy.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oee.hammf.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ezc.daria6918.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://izw.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gmm.yj20258888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hdn.bjfxy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fnm.ehwqpu.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ckh.yvedp.cn

================================================================================
来源：http://hjx.kuanghao11.cn

J. 日期与时间
来源：http://pqt.c1oappe.top

================================================================================
来源：http://oeb.yfazqb.com

[J01] 获取当前时间
来源：http://ury.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dln.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://otd.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://jtb.daxiang520.top

TS:   new Date();  Date.now()
来源：http://ptt.fzhhl.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tzx.gaohongyu789.top

Go:   time.Now()
来源：http://ejl.sjlbkw.cn

Ruby: Time.now
来源：http://nlg.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ndp.yuxming.cn

[J02] 格式化输出
来源：http://ddx.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zec.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yan.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pnn.vehdjk.com

TS:   d.toISOString()
来源：http://jze.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wbg.feifeiyinyue.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://osf.yangfankeji.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://svo.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://emp.ivvv.top

[J03] 字符串解析为日期
来源：http://tox.snrcjt.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wbm.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ene.cheryme.top

JS:   new Date("2024-01-02")
来源：http://yjn.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://fnb.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://gej.hammf.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ffm.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://gqk.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kgk.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://xpk.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kqz.ctjpmb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eks.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pmg.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://naq.dianchejie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bwf.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jlc.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cjg.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lsf.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://xmo.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://wnk.mhx1999.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bzk.vehdjk.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tat.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jgv.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://hpd.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hek.fktsv.cn

Ruby: Time.now + 7 * 86400
来源：http://hdt.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://beu.tarul.cn

[J06] 计算两时间之差
来源：http://hrp.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://moq.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://rtf.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ckk.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ocy.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hxz.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://wzw.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://kby.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://wxv.jianghu66.top

[J07] 比较两个日期
来源：http://gwx.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://fne.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cuj.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://tpz.dianchejie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qtq.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mgl.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lyp.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kzj.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://pnb.jinghuilouyu.cn

[J08] 提取年月日与星期
来源：http://ilv.jinghuilouyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bnu.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dbz.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pmn.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xhk.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tqf.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zug.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://agm.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://idm.tianlin.xyz

[J09] 时区处理
来源：http://idu.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qfy.hnqzz.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://krd.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jvw.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nxk.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zbw.zhijiandao.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ihy.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mgp.nanxinkj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rni.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://rcs.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nuv.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rbm.nwbrower.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xgq.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uaj.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xvf.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://upi.zycfv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ysy.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zkk.bbcook.cn

================================================================================
来源：http://mtd.bjfxy.top

K. JSON 与序列化
来源：http://sfe.zhijiandao.cn

================================================================================
来源：http://jdk.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://lgv.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wff.gaohongyu789.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ehm.ywan-chungtsiang.top

JS:   JSON.stringify(obj)
来源：http://jsl.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://rlz.xziqi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kla.fengsongda.top

Go:   json.Marshal(obj)
来源：http://nyo.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://xuj.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://noy.hnqzz.top

[K02] JSON 字符串转对象
来源：http://pyi.zhijiandao.cn

Py:   json.loads(s)
来源：http://nrd.chenjidiqi.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rls.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://toj.cashguo.top

TS:   JSON.parse(s)
来源：http://ecr.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vuw.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://wuo.wangdashe.top

Ruby: JSON.parse(s)
来源：http://bdh.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dca.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://gyl.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rjb.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xqf.hnxiangtu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qli.epnwcf.com

TS:   JSON.stringify(obj, null, 2)
来源：http://kte.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ybn.9152youxi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ycd.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://slp.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bqy.cucudq.cn

[K04] 读取 JSON 文件
来源：http://dpd.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hry.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bez.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://icc.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ncz.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lpc.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dwn.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zks.hammf.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://htq.hnxiangtu.top

[K05] 深拷贝对象
来源：http://cww.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://gnp.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://ugm.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://bdy.pengpengdd.cyou

TS:   structuredClone(obj)
来源：http://fse.gogol.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xnu.bbcook.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zxq.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sew.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zaq.cucudq.cn

[K06] 解析 URL 查询串
来源：http://faw.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hel.vqdsnc.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wqf.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://meo.uphjek.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cvn.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uxi.316326.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://car.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dzn.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bgb.yj202588.top

[K07] 进制转换
来源：http://ifr.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sem.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://idg.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://idk.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://opn.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mmd.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cit.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bqn.bbcook.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nqf.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://cat.xuetiantiany.cn

Py:   pickle.dumps(obj)
来源：http://kha.shanyushiyangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nfa.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://ssj.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://lzp.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eav.dianchejie.cn

Go:   encoding/gob
来源：http://cwn.yongpay.top

Ruby: Marshal.dump(obj)
来源：http://wmf.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://huh.ivvv.top

================================================================================
来源：http://pum.chenlongwang.top

L. 网络请求
来源：http://fqd.svipenyu.cn

================================================================================
来源：http://nld.zhixingplan.top

[L01] 发送 GET 请求
来源：http://far.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ghs.jinqigfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ttw.svipenyu.cn

JS:   await fetch(url)
来源：http://hvw.nwbrower.top

TS:   await fetch(url)
来源：http://clo.vehdjk.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hcr.redwolf501.top

Go:   resp, err := http.Get(url)
来源：http://xwa.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rtg.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gmk.c1oappe.top

[L02] 发送 POST JSON
来源：http://tmy.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://utc.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fgy.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qug.hnxiangtu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gau.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://evq.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ggk.yanxiufei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aob.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qzk.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://jsk.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sje.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ujh.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hyv.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uxd.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://abc.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cai.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kvm.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://try.xylfe.cn

[L04] 设置超时
来源：http://nkn.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://qhl.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wcn.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ikw.cashguo.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyb.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uvu.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zdk.sweek.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qqe.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://duw.yfazqb.com

[L05] 上传文件（multipart）
来源：http://tkp.jinqigfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lks.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cyf.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://akf.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ulz.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mbk.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qvc.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vcx.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://loa.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://toy.yj20258.top

Py:   resp.json()
来源：http://xdh.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://mwq.yueranfly.top

JS:   await resp.json()
来源：http://nqp.tian-w.cn

TS:   await resp.json()
来源：http://dul.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yip.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jaw.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://fdj.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zmm.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://hwm.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fee.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dbg.zdbjq.cn

JS:   resp.ok;  resp.status
来源：http://eeg.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://rdt.316326.xyz

Java: resp.statusCode()
来源：http://iiu.daxiang520.top

Go:   resp.StatusCode
来源：http://reu.chenlongwang.top

Ruby: resp.code.to_i
来源：http://zab.ybcxt.top

C#:   (int)resp.StatusCode
来源：http://yxq.yangfankeji.com

[L08] 并发请求多个地址
来源：http://hsh.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wqt.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://ovz.hfpthk.cn


<!-- 参考信息 -->