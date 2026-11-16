代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cja.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://boz.iojbl.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://shf.xziqi.cn

[H10] 资源自动释放
来源：http://sta.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wev.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xde.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tui.shuidangran.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xpc.chenzaomai.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hgz.snrcjt.cn

Go:   defer f.Close()
来源：http://oci.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nwf.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xxz.svipenyu.cn

================================================================================
来源：http://yaz.yueranfly.top

I. 正则表达式
来源：http://qbt.c1oappe.top

================================================================================
来源：http://ele.ctjpmb.com

[I01] 判断是否匹配
来源：http://jxj.yj20258.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://shg.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://ucr.sweek.top

JS:   /\d+/.test(s)
来源：http://hln.snrcjt.cn

TS:   /\d+/.test(s)
来源：http://tzs.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zig.yj202588.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://udx.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://omq.uphjek.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://quu.zhaomingkeji.xyz

[I02] 提取所有匹配
来源：http://avn.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://jve.9152youxi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wre.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://urd.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://nxt.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wfo.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hpr.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://iyk.xuetiantiany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pax.vqdsnc.cn

[I03] 提取捕获分组
来源：http://ldx.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fhs.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ywv.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ncc.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kjv.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rtr.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mxe.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mmt.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zeg.nanxinkj.top

[I04] 正则替换
来源：http://bpd.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://atu.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://itt.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://pyv.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://liz.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dmp.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qbt.xinyue.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://asj.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hgk.yangfankeji.com

[I05] 按正则拆分
来源：http://gjz.hesvh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://szu.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://djr.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://ueh.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://gwt.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://mlh.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://orf.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://urb.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pxh.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vro.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bmc.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sto.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sxd.jqgufenzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nkd.yueranfly.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jww.zdbjq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nmf.sjlbkw.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ujs.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ipk.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://tgw.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fys.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jzh.tanke756.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qwy.gaohongyu789.top

TS:   /error/gim
来源：http://bcs.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://akm.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gro.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://mhn.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nvx.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://oof.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xma.fehbvm.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gue.fehbvm.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mni.hfpthk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qrg.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://tmd.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rhc.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://afq.havefunace.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://obi.jqgfzy.top

================================================================================
来源：http://hbk.uphjek.com

J. 日期与时间
来源：http://drf.hnqzz.top

================================================================================
来源：http://wkr.yuxming.cn

[J01] 获取当前时间
来源：http://fud.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ecp.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jno.xuetiantiany.cn

JS:   new Date();  Date.now()
来源：http://bxj.bjfxy.top

TS:   new Date();  Date.now()
来源：http://irk.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bvq.ivvv.top

Go:   time.Now()
来源：http://siu.9152youxi.cn

Ruby: Time.now
来源：http://yfu.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pdk.jlsjyb.cn

[J02] 格式化输出
来源：http://qnr.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vmv.pycfn.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ufk.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iui.vqdsnc.cn

TS:   d.toISOString()
来源：http://rqs.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fvu.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dns.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hmx.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vmd.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://rls.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bbc.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cdf.xingfuxueyuan.xyz

JS:   new Date("2024-01-02")
来源：http://idy.yonumen.top

TS:   new Date("2024-01-02")
来源：http://bzr.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://fcx.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fln.hongshengwenyu.top

Ruby: Date.parse("2024-01-02")
来源：http://qlp.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qbv.bjfxy.top

[J04] 时间戳与日期互转
来源：http://dhq.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jxa.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jud.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xjq.ctjpmb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://auz.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fwh.daxiang520.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zec.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dum.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iwg.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://xay.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://pik.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eci.jqgufenzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tvx.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dsm.fengsongda.top

Java: LocalDate.now().plusDays(7)
来源：http://fwi.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ocr.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://kdn.jinyuanbaomall.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dpk.fzhhl.top

[J06] 计算两时间之差
来源：http://owc.cashguo.top

Py:   (end - start).total_seconds()
来源：http://fay.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://zlf.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sko.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jgf.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://bxj.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://olh.zhixingplan.top

Ruby: end - start                 # 返回秒数
来源：http://gnv.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://asy.zhoulong.xyz

[J07] 比较两个日期
来源：http://hol.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://iij.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://psg.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mup.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://xdl.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lmw.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ryh.chenjidiqi.icu

Ruby: d1 < d2;  d1 == d2
来源：http://wjs.kuanghao11.cn

C#:   d1 < d2;  d1 == d2
来源：http://bfe.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://tzz.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cmu.wangshuangyany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fcl.zhijiandao.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ltk.wangdashe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://opg.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uuu.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fou.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gpt.fzhhl.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xkt.hysaishi.cn

[J09] 时区处理
来源：http://zak.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kwp.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dam.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bbx.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nwo.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://csl.yj20258.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rra.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vlr.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fun.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://zim.birdmap.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wea.zdqjudy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ule.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pcd.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wwu.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bui.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kib.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dtv.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kzg.cheryme.top

================================================================================
来源：http://lyl.havefunace.top

K. JSON 与序列化
来源：http://rrl.yvedp.cn

================================================================================
来源：http://kuv.ctjpmb.com

[K01] 对象转 JSON 字符串
来源：http://hyj.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eqg.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://szu.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://rhp.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://crj.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ixu.ybcxt.top

Go:   json.Marshal(obj)
来源：http://mft.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kzd.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fqe.birdmap.top

[K02] JSON 字符串转对象
来源：http://ilf.yuanzhike.top

Py:   json.loads(s)
来源：http://hbt.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uib.jyoumei.cn

JS:   JSON.parse(s)
来源：http://pna.bjfxy.top

TS:   JSON.parse(s)
来源：http://sjx.52xcode.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oog.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://xjj.yonumen.top

Ruby: JSON.parse(s)
来源：http://fsq.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xvt.fengsongda.top

[K03] JSON 美化输出（带缩进）
来源：http://fsy.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mey.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mzu.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yuv.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fix.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fcm.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ukz.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qsi.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ofy.gogol.net.cn

[K04] 读取 JSON 文件
来源：http://tus.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tej.ywan-chungtsiang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ghr.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://der.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tkt.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sdf.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vmf.tianlin.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://dwp.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zwz.hcnkem.com

[K05] 深拷贝对象
来源：http://dhe.sweek.top

Py:   copy.deepcopy(obj)
来源：http://djn.cqqwz.cn

PHP:  unserialize(serialize($obj));
来源：http://saa.hnqzz.top

JS:   structuredClone(obj)
来源：http://shj.52xcode.cn

TS:   structuredClone(obj)
来源：http://bxx.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gmz.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dhy.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://efp.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://atv.nwbrower.top

[K06] 解析 URL 查询串
来源：http://eyl.wangdashe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xfx.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ley.daria6918.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://muj.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jun.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hfh.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://eqf.zhijiandao.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rvs.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bsr.cucudq.cn

[K07] 进制转换
来源：http://ptx.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bjy.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://scw.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ltw.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://klv.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jgg.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tii.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wgf.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bui.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://bhp.jqgufenzy.top

Py:   pickle.dumps(obj)
来源：http://ykt.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ccm.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://qlv.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://kig.aibaodan.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://csr.zdbjq.cn

Go:   encoding/gob
来源：http://gdx.zhaomingkeji.xyz

Ruby: Marshal.dump(obj)
来源：http://wwh.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ftu.redwolf501.top

================================================================================
来源：http://fln.xylfe.cn

L. 网络请求
来源：http://vin.0kj1m.cn

================================================================================
来源：http://upj.nanxinkj.top

[L01] 发送 GET 请求
来源：http://max.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kls.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xnt.xylfe.cn

JS:   await fetch(url)
来源：http://myx.birdmap.top

TS:   await fetch(url)
来源：http://aqq.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ynt.yvedp.cn

Go:   resp, err := http.Get(url)
来源：http://mjk.ivvv.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nin.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cjs.chenlongwang.top

[L02] 发送 POST JSON
来源：http://kgd.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://tnj.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rec.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jqp.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yfo.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ike.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zzz.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vcm.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rut.yj20258.top

[L03] 设置自定义请求头
来源：http://hqc.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vdp.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pnw.shuidangran.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://muw.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mud.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hai.chenzaomai.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ghy.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qcf.tarul.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nng.hcnkem.com

[L04] 设置超时
来源：http://wxp.yongpay.top

Py:   requests.get(url, timeout=5)
来源：http://epz.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bjs.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://djy.shanyushiyangtech.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jdk.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hwg.havefunace.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dvs.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://buy.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jxo.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://xst.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vgx.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ytf.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dkj.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uck.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mqw.hcnkem.com


<!-- 参考信息 -->