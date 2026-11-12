代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://suk.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fuw.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://noh.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://orb.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://euv.quarkkingdee.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dfs.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://peu.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fgj.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ceq.gotoacloud.top

Go:   defer f.Close()
来源：http://vbb.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bfj.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tyi.havefunace.top

================================================================================
来源：http://rqn.yongpay.top

I. 正则表达式
来源：http://xbr.ivvv.top

================================================================================
来源：http://itc.zhoulong.xyz

[I01] 判断是否匹配
来源：http://rvw.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ozx.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://qpn.fehbvm.com

JS:   /\d+/.test(s)
来源：http://dib.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://iwl.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ibn.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aam.hfpthk.cn

Ruby: s.match?(/\d+/)
来源：http://tui.pycfn.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aqo.yangfankeji.com

[I02] 提取所有匹配
来源：http://vrl.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://kjj.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xbx.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kjn.ehwqpu.com

TS:   s.match(/\d+/g)
来源：http://frr.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aef.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vkl.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://awt.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rme.c1oappe.top

[I03] 提取捕获分组
来源：http://biw.ydzc1.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ahr.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xqw.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ocv.gotoacloud.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sxk.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gtu.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wbb.kuanghao11.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zrf.andypj.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lfm.jinqigufen.top

[I04] 正则替换
来源：http://mgf.aizwys.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yhm.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aco.xinyue.icu

JS:   s.replace(/\d+/g, "#")
来源：http://duj.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://shs.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uzy.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vzk.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rkx.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://irx.sweek.top

[I05] 按正则拆分
来源：http://hix.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mmm.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://imp.andypj.xyz

JS:   s.split(/\s*,\s*/)
来源：http://tqi.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://wox.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://dag.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sbk.andypj.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://mxs.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lyb.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lbx.zycfv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baa.meibo888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yqi.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rtv.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wpm.smart0.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ctf.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ghl.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mcp.hnxiangtu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ikv.haohaochexian.top

[I07] 忽略大小写与多行模式
来源：http://zyp.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ryg.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qpa.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xkv.yuanzhike.top

TS:   /error/gim
来源：http://flk.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rnm.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cuq.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://ebr.pengpengdd.cyou

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tra.fzhhl.top

[I08] 贪婪与非贪婪匹配
来源：http://fut.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jcs.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ffd.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uje.hywenlv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dxr.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fyq.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kov.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ejg.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dth.hywenlv.cn

================================================================================
来源：http://uzi.yanxiufei.cn

J. 日期与时间
来源：http://tbo.dianchejie.cn

================================================================================
来源：http://gbi.nanxuanxn.top

[J01] 获取当前时间
来源：http://pau.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wtc.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://njm.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://opy.jinyuanbaomall.cn

TS:   new Date();  Date.now()
来源：http://yhp.fanxiaobao.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://qil.hysaishi.cn

Go:   time.Now()
来源：http://lpg.hywenlv.cn

Ruby: Time.now
来源：http://ana.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ozy.zdbjq.cn

[J02] 格式化输出
来源：http://fnc.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nqx.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cqy.xinyue.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mqs.pycfn.com

TS:   d.toISOString()
来源：http://xse.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://okt.jyoumei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mop.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iwe.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://slo.jinqigufen.top

[J03] 字符串解析为日期
来源：http://vqg.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xqg.cqqwz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ual.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://epm.ivvv.top

TS:   new Date("2024-01-02")
来源：http://tue.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://ujh.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://moz.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://cwt.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fre.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://uke.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qvf.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rkv.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nlt.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kzv.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://duj.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nby.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zmo.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zog.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://hzp.yj202588.top

Py:   now + timedelta(days=7)
来源：http://niu.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yqc.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mmv.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ibd.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://wmc.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xae.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://hil.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://leq.zhijiandao.cn

[J06] 计算两时间之差
来源：http://hjn.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://tvt.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://spa.epnwcf.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gsg.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lyl.nanxuanxn.top

Java: Duration.between(start, end).toSeconds()
来源：http://nkg.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://azs.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://vqh.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://odg.sxryk.cn

[J07] 比较两个日期
来源：http://jdh.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://mcr.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yyc.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://rlz.yongpay.top

TS:   d1.getTime() < d2.getTime()
来源：http://ryg.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://grp.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bcb.bjfxy.top

Ruby: d1 < d2;  d1 == d2
来源：http://rka.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://dqd.bbcook.cn

[J08] 提取年月日与星期
来源：http://beq.zycfv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ekd.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rkx.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pqy.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oil.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wtf.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rsw.aibaodan.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ltl.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cbd.yj20258888.top

[J09] 时区处理
来源：http://jce.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ltd.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tck.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ruv.zhengqikj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bqj.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vxi.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sex.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vtt.tianlin.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bvi.yuxming.cn

[J10] 取今天 / 本月第一天
来源：http://qyx.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rlm.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ike.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ukg.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kat.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uee.yfazqb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hzu.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://etm.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mgc.meibo888.top

================================================================================
来源：http://cmd.ivvv.top

K. JSON 与序列化
来源：http://cpq.nanxinkj.top

================================================================================
来源：http://ofn.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://hnn.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eow.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rjt.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://fjt.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://knt.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://znj.ppjwa.cn

Go:   json.Marshal(obj)
来源：http://nrl.yuxming.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nvv.dashuyun.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eti.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://clu.ehwqpu.com

Py:   json.loads(s)
来源：http://qmg.sweek.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dzl.hysaishi.cn

JS:   JSON.parse(s)
来源：http://rvu.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://emp.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://byh.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://mqq.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://prl.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iwo.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://vlf.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kqd.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dab.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zxs.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://lwr.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://erj.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rnm.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://fxr.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rkk.meibo888.top

[K04] 读取 JSON 文件
来源：http://tab.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dks.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sqz.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://trp.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zqu.pycfn.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ihh.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ano.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ejp.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jvb.0kj1m.cn

[K05] 深拷贝对象
来源：http://snv.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://bgg.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://rkg.yvedp.cn

JS:   structuredClone(obj)
来源：http://nid.sysykeji.top

TS:   structuredClone(obj)
来源：http://gkw.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qfe.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://geh.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ucm.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://plw.uphjek.com

[K06] 解析 URL 查询串
来源：http://yuc.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bxb.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bht.dashuyun.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mjw.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ioi.zdbjq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qae.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nya.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://feg.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wyp.0kj1m.cn

[K07] 进制转换
来源：http://vhc.0kj1m.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sjs.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gcf.mhx1999.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zfx.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tgr.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xry.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yvo.vqdsnc.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xkx.jinyuanbaomall.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aay.quarkkingdee.top

[K08] 二进制序列化（非 JSON）
来源：http://lax.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://tqn.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://gaj.ydzc1.top

JS:   v8.serialize(obj)        // Node
来源：http://jdj.ybcxt.top

TS:   v8.serialize(obj)        // Node
来源：http://jtp.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hsd.zdqjudy.top

Go:   encoding/gob
来源：http://ndl.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://xwo.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zea.shangyingyoupin.top

================================================================================
来源：http://zck.birdmap.top

L. 网络请求
来源：http://yce.hesvh.cn

================================================================================
来源：http://ozt.hnqzz.top

[L01] 发送 GET 请求
来源：http://jty.hesvh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tqi.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://scs.hnqzz.top

JS:   await fetch(url)
来源：http://ihx.hysaishi.cn

TS:   await fetch(url)
来源：http://zbn.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ddu.nwbrower.top

Go:   resp, err := http.Get(url)
来源：http://foy.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qsa.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pws.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://jte.hywenlv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zmy.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iid.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pkw.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://abe.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oey.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eeb.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tvu.zhengqikj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://igk.zdbjq.cn

[L03] 设置自定义请求头
来源：http://fww.zycfv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jpl.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://whd.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://flf.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zdq.havefunace.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mmu.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gus.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xdd.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aft.bbcook.cn

[L04] 设置超时
来源：http://coe.iojbl.cn

Py:   requests.get(url, timeout=5)
来源：http://aew.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zvz.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zpq.svipenyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rst.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uwf.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pad.9152youxi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qwf.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rzr.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://pre.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dya.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wrv.wangshuangyany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ezo.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fnd.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://svp.zhongyouzk.top


<!-- 参考信息 -->