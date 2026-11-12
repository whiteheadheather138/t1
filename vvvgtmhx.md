代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nln.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qrl.redwolf501.top

C#:   // 自定义异常类中加 Code 属性
来源：http://atg.ppjwa.cn

[H10] 资源自动释放
来源：http://tzv.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wzt.ydjk.org.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nfo.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://quy.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uos.daria6918.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zgs.ctjpmb.com

Go:   defer f.Close()
来源：http://lap.hnxiangtu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xoh.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fcr.daria6918.cn

================================================================================
来源：http://oxu.ywan-chungtsiang.top

I. 正则表达式
来源：http://qpm.kuanghao11.cn

================================================================================
来源：http://qhx.fzhhl.top

[I01] 判断是否匹配
来源：http://lkn.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rxl.redwolf501.top

PHP:  preg_match('/\d+/', $s);
来源：http://xkz.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://lig.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://gco.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ncn.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wjj.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://psm.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jnj.xuanzx.com

[I02] 提取所有匹配
来源：http://plx.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://onk.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dks.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tof.chenzaomai.com

TS:   s.match(/\d+/g)
来源：http://fsp.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pgi.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://urp.hongshengwenyu.top

Ruby: s.scan(/\d+/)
来源：http://toz.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lqy.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://lmo.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yyk.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qyt.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kme.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://byi.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wpk.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://udy.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bnk.bjfxy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qvf.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://pyy.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jwe.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jsh.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://joj.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://olm.shanyushiyangtech.top

Java: s.replaceAll("\\d+", "#")
来源：http://enw.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://oig.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://bao.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bij.316326.xyz

[I05] 按正则拆分
来源：http://bcg.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sda.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://squ.tarul.cn

JS:   s.split(/\s*,\s*/)
来源：http://jwo.zhixingplan.top

TS:   s.split(/\s*,\s*/)
来源：http://wbp.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://arb.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://woc.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://stn.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zdv.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cdl.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://poz.tarul.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wtc.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://krg.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aoz.aibaodan.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uyf.yueranfly.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yiz.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fzc.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://orn.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://ecn.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wgl.guannengcc.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://stm.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ysb.zdbjq.cn

TS:   /error/gim
来源：http://ahf.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yme.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ith.redwolf501.top

Ruby: s.scan(/error/i)
来源：http://zcb.aizwys.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lco.hnxiangtu.top

[I08] 贪婪与非贪婪匹配
来源：http://zxs.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lrp.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://too.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pgr.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mgt.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://arx.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kxk.guowangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kza.kuanghao11.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rxg.vehdjk.com

================================================================================
来源：http://czl.fanxiaobao.xyz

J. 日期与时间
来源：http://ncq.hfpthk.cn

================================================================================
来源：http://cpy.yanxiufei.cn

[J01] 获取当前时间
来源：http://sgo.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://olp.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rdw.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://evq.hfpthk.cn

TS:   new Date();  Date.now()
来源：http://znt.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ckq.ehwqpu.com

Go:   time.Now()
来源：http://qbl.52xcode.cn

Ruby: Time.now
来源：http://xgl.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zbs.snrcjt.cn

[J02] 格式化输出
来源：http://hel.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://unt.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fip.smart0.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://grg.shangyingyoupin.top

TS:   d.toISOString()
来源：http://jyc.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sdu.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wyz.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mks.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://unq.nwbrower.top

[J03] 字符串解析为日期
来源：http://thh.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zzt.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ase.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://spm.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://ohi.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://sii.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hzc.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://jtg.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mje.wangdashe.top

[J04] 时间戳与日期互转
来源：http://ctk.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ftv.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hhv.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ijr.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://edb.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qcs.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ajk.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://irw.sufxvd.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hdb.ydjk.org.cn

[J05] 时间加减（加 7 天）
来源：http://wws.chenjidiqi.icu

Py:   now + timedelta(days=7)
来源：http://qqq.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hzd.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://neh.ydjk.org.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qqq.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://zyk.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pqo.bjfxy.top

Ruby: Time.now + 7 * 86400
来源：http://tks.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://ugk.tian-w.cn

[J06] 计算两时间之差
来源：http://rff.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://kmp.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://nzc.chenlongwang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tim.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://phd.0kj1m.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zxq.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://njn.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://qhb.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://kvs.gzhubu.top

[J07] 比较两个日期
来源：http://rhb.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://mva.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eev.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://cav.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wse.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sci.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nab.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://yld.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://ipb.birdmap.top

[J08] 提取年月日与星期
来源：http://ugd.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://laa.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cqa.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sdv.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xjx.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nll.guowangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://laf.shanyushiyangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zel.c1oappe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://shy.zycfv.cn

[J09] 时区处理
来源：http://olu.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rjw.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dld.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kyo.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rmb.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xcd.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yym.cashguo.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nan.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pzx.hongshengwenyu.top

[J10] 取今天 / 本月第一天
来源：http://prk.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vxo.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jsj.nwbrower.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mlt.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eef.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bdl.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yld.aizwys.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zmp.cucudq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yvp.yfazqb.com

================================================================================
来源：http://vay.nanxinkj.top

K. JSON 与序列化
来源：http://xki.uphjek.com

================================================================================
来源：http://gfs.vehdjk.com

[K01] 对象转 JSON 字符串
来源：http://gzz.vqdsnc.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ijz.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xui.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://hpy.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://llx.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nbf.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://arm.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mmw.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xrb.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://meg.bbcook.cn

Py:   json.loads(s)
来源：http://evc.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fge.iojbl.cn

JS:   JSON.parse(s)
来源：http://kcy.daxiang520.top

TS:   JSON.parse(s)
来源：http://yzr.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lsz.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://myk.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://ttz.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://skd.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://gsf.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ubq.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bql.yvedp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wec.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qpt.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nyh.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cpx.yuanzhike.top

Ruby: JSON.pretty_generate(obj)
来源：http://ldb.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nft.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://xan.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://liy.yanxiufei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gfk.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ohv.52xcode.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cju.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gjl.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jfk.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://izj.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wba.aizwys.cn

[K05] 深拷贝对象
来源：http://loq.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://mlz.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://qde.fengsongda.top

JS:   structuredClone(obj)
来源：http://zlw.nanxinkj.top

TS:   structuredClone(obj)
来源：http://dcv.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hdx.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mew.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yff.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yqy.gzhubu.top

[K06] 解析 URL 查询串
来源：http://fzi.yvedp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sih.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kyc.hywenlv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wuz.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tge.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mpk.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zss.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://srs.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cpg.gotoacloud.top

[K07] 进制转换
来源：http://nlm.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kfz.shanyushiyangtech.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yed.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://smu.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kkq.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ztu.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vrn.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lmd.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ynr.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://uvo.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://rwy.xuanzx.com

PHP:  serialize($obj);  unserialize($s);
来源：http://lva.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://gww.zhengqikj.top

TS:   v8.serialize(obj)        // Node
来源：http://khx.nanxinkj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ygl.sysykeji.top

Go:   encoding/gob
来源：http://uik.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://uly.jinqigufen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fyw.smart0.xyz

================================================================================
来源：http://hbe.aizwys.cn

L. 网络请求
来源：http://jrn.ppjwa.cn

================================================================================
来源：http://eqi.wangdashe.top

[L01] 发送 GET 请求
来源：http://hqq.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ihx.hcnkem.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mro.tanke756.top

JS:   await fetch(url)
来源：http://ece.hnxiangtu.top

TS:   await fetch(url)
来源：http://omv.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://het.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://pqx.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ump.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pun.yueranfly.top

[L02] 发送 POST JSON
来源：http://tlk.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bdh.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jip.tanke756.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ycp.svipenyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cnw.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ytd.guowangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qbg.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xjs.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://czq.cashguo.top

[L03] 设置自定义请求头
来源：http://jkt.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xll.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cyd.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hhs.fzhhl.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dtt.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://chg.gzhubu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tba.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rde.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jrw.sxryk.cn

[L04] 设置超时
来源：http://bef.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://hfi.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rmt.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sqb.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hfr.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bml.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fdc.yfazqb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rwm.shuidangran.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mdy.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://lvn.chenzaomai.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dto.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jdl.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sdi.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fop.aibaodan.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fss.wangshuangyany.cn


<!-- 参考信息 -->