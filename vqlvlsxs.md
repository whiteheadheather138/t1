代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://afm.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jtz.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uzj.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bgf.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://msj.tarul.cn

Go:   defer f.Close()
来源：http://lfa.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zzx.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bnl.hcnkem.com

================================================================================
来源：http://fyv.hfpthk.cn

I. 正则表达式
来源：http://amj.dianchejie.cn

================================================================================
来源：http://iao.havefunace.top

[I01] 判断是否匹配
来源：http://ewr.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wmm.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://atk.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://jcy.c1oappe.top

TS:   /\d+/.test(s)
来源：http://trt.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://utt.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ysc.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://cxh.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sgr.chenlongwang.top

[I02] 提取所有匹配
来源：http://wjm.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://ual.hcnkem.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://awz.iojbl.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://see.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://nlw.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xep.yueranfly.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zdp.epnwcf.com

Ruby: s.scan(/\d+/)
来源：http://mts.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://krl.yfazqb.com

[I03] 提取捕获分组
来源：http://yns.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://quv.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wyl.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://phl.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uny.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xwv.shzxlz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mtw.zdqjudy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ogl.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://elf.52xcode.cn

[I04] 正则替换
来源：http://yel.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oqb.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://laq.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://gbz.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://kgk.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mui.shangyingyoupin.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rzh.tarul.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fic.shzxlz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jop.yanxiufei.cn

[I05] 按正则拆分
来源：http://wms.wangdashe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gjx.daria6918.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://smr.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://kdm.yuxming.cn

TS:   s.split(/\s*,\s*/)
来源：http://yzi.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://ubc.iojbl.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dvv.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://suw.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lld.hnqzz.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wiu.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://suu.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qqb.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ceq.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blh.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aut.xinyue.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mxx.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hdb.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wwv.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://urk.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pbf.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nho.zdqjudy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://izn.jinqigfzy.top

TS:   /error/gim
来源：http://pkp.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bhu.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ylt.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://gjj.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ikh.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://hjv.yonumen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sdp.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jiq.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pgf.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://upp.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cri.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uob.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oyi.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hsf.ywan-chungtsiang.top

================================================================================
来源：http://ijq.xuetiantiany.cn

J. 日期与时间
来源：http://bfo.zhaomingkeji.xyz

================================================================================
来源：http://dpc.xinyue.icu

[J01] 获取当前时间
来源：http://huu.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eqc.gogol.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sjk.yuxming.cn

JS:   new Date();  Date.now()
来源：http://onm.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://sda.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yzh.jlsjyb.cn

Go:   time.Now()
来源：http://vyy.jqgfzy.top

Ruby: Time.now
来源：http://enz.tianlin.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://onl.hammf.cn

[J02] 格式化输出
来源：http://rpq.jyoumei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qhk.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qnn.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mrc.ydzc1.top

TS:   d.toISOString()
来源：http://hpv.uphjek.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qyy.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hic.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://krn.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://loi.aizwys.cn

[J03] 字符串解析为日期
来源：http://slp.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yrm.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pwd.cashguo.top

JS:   new Date("2024-01-02")
来源：http://hov.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://noo.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://gev.hnqzz.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jjj.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://ota.yj202588.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wah.yongpay.top

[J04] 时间戳与日期互转
来源：http://hyt.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gss.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lno.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://abp.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rwe.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rij.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pll.xziqi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lfn.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qab.aizwys.cn

[J05] 时间加减（加 7 天）
来源：http://olz.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://cxf.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qri.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ise.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vgz.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://yxf.snrcjt.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dxy.dashuyun.cn

Ruby: Time.now + 7 * 86400
来源：http://xat.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://psc.shzxlz.cn

[J06] 计算两时间之差
来源：http://erj.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://fmi.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://lkp.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wcj.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hjy.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ipt.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://vgl.ywan-chungtsiang.top

Ruby: end - start                 # 返回秒数
来源：http://iaq.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://apd.shzxlz.cn

[J07] 比较两个日期
来源：http://ldn.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://xxj.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xko.ctjpmb.com

JS:   d1.getTime() < d2.getTime()
来源：http://tzc.daria6918.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pvr.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://myz.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bjx.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://zdy.nanxinkj.top

C#:   d1 < d2;  d1 == d2
来源：http://wwx.uphjek.com

[J08] 提取年月日与星期
来源：http://sqd.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vlx.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tpk.dashuyun.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zpi.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vbz.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zhp.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wfs.chenzaomai.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rij.sweek.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qqp.hywenlv.cn

[J09] 时区处理
来源：http://byd.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uaz.chenjidiqi.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ilu.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lrr.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ghz.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rnt.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://umj.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://efj.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://upj.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://sgm.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bdh.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rkw.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jtr.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dtc.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nkn.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lwi.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zyt.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bzn.xuetiantiany.cn

================================================================================
来源：http://wqa.aibaodan.cn

K. JSON 与序列化
来源：http://tio.cashguo.top

================================================================================
来源：http://ryj.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://shq.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sxj.kuanghao11.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eqn.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://fcd.yj202588.top

TS:   JSON.stringify(obj)
来源：http://him.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jzo.ydjk.org.cn

Go:   json.Marshal(obj)
来源：http://mmr.cqqwz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ihq.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zgq.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://kps.gaohongyu789.top

Py:   json.loads(s)
来源：http://hew.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ghw.andypj.xyz

JS:   JSON.parse(s)
来源：http://hos.vehdjk.com

TS:   JSON.parse(s)
来源：http://orm.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://srp.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://dtk.hcnkem.com

Ruby: JSON.parse(s)
来源：http://lwe.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qke.316326.xyz

[K03] JSON 美化输出（带缩进）
来源：http://idx.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sxc.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uib.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://umc.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rdi.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oth.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wnf.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://gkf.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iii.pycfn.com

[K04] 读取 JSON 文件
来源：http://snu.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://koo.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://twv.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://prs.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gfe.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eph.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ecd.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://grn.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xvm.pycfn.com

[K05] 深拷贝对象
来源：http://ggl.sufxvd.cn

Py:   copy.deepcopy(obj)
来源：http://ajj.havefunace.top

PHP:  unserialize(serialize($obj));
来源：http://jrk.yj202588.top

JS:   structuredClone(obj)
来源：http://ckj.yongpay.top

TS:   structuredClone(obj)
来源：http://uyv.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mum.yueranfly.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://amf.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wzc.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uwk.bbcook.cn

[K06] 解析 URL 查询串
来源：http://clk.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kco.hfpthk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://swm.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tta.yangfankeji.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://box.haohaochexian.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xva.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://inh.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dho.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://egb.shzxlz.cn

[K07] 进制转换
来源：http://nim.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jxc.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ral.mhx1999.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dlq.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cvn.jqgufenzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rfx.hfpthk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ucm.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dtw.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jhz.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://wjs.hnqzz.top

Py:   pickle.dumps(obj)
来源：http://qbs.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iea.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://xpq.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://fzb.sweek.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mlp.xinyue.icu

Go:   encoding/gob
来源：http://rmq.xuanzx.com

Ruby: Marshal.dump(obj)
来源：http://jzx.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pxe.wangdashe.top

================================================================================
来源：http://zlo.316326.xyz

L. 网络请求
来源：http://xar.xziqi.cn

================================================================================
来源：http://srk.yj20258888.top

[L01] 发送 GET 请求
来源：http://wpl.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wqo.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nzv.yuxming.cn

JS:   await fetch(url)
来源：http://ius.hysaishi.cn

TS:   await fetch(url)
来源：http://med.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rob.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://zbr.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://dgs.chenjidiqi.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wrz.gaohongyu789.top

[L02] 发送 POST JSON
来源：http://vci.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://nsi.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://des.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://euy.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cyu.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tnj.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jvb.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://azw.zdqjudy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cfc.mhx1999.top

[L03] 设置自定义请求头
来源：http://btn.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bcj.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ihe.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uej.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iso.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://shg.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jwe.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zwn.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iyn.xuetiantiany.cn

[L04] 设置超时
来源：http://uzm.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://fuk.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://obr.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zya.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cmy.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ovk.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cdx.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://asr.gzhubu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qrs.cucudq.cn

[L05] 上传文件（multipart）
来源：http://zbs.yuanzhike.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dts.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aqh.yfazqb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fwf.shanyushiyangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kcm.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bae.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eud.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jpd.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gej.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://dln.jinghuilouyu.cn


<!-- 参考信息 -->