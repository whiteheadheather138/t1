代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lam.havefunace.top

Go:   defer f.Close()
来源：http://zsm.kuanghao11.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ghv.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ihf.aibaodan.cn

================================================================================
来源：http://ite.wangshuangyany.cn

I. 正则表达式
来源：http://tot.cqqwz.cn

================================================================================
来源：http://yvf.nanxuanxn.top

[I01] 判断是否匹配
来源：http://sye.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mhy.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://cfn.sweek.top

JS:   /\d+/.test(s)
来源：http://mda.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://xwu.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gbn.yongpay.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ggk.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://png.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bpm.hnqzz.top

[I02] 提取所有匹配
来源：http://dtt.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://lbt.jianghu66.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tjf.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uhu.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://ues.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mkz.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nzv.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://mdr.yj20258888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hnf.birdmap.top

[I03] 提取捕获分组
来源：http://bpu.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ofj.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bld.shanyushiyangtech.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xil.dianchejie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uep.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iyb.sweek.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mme.9152youxi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gpb.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bpu.zhijiandao.cn

[I04] 正则替换
来源：http://zmv.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zcy.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://trk.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tzz.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://szr.shangyingyoupin.top

Java: s.replaceAll("\\d+", "#")
来源：http://ayx.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ohv.nanxuanxn.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hlg.jyoumei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dsq.chenjidiqi.icu

[I05] 按正则拆分
来源：http://rai.wangdashe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tnc.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ois.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://fpf.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://oeh.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://ocr.dianchejie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wsb.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fjm.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hpk.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://umd.daria6918.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qmd.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gqw.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hut.hcnkem.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uoj.andypj.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wty.sufxvd.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kqz.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://plw.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qby.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://lok.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cco.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://say.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hnx.pycfn.com

TS:   /error/gim
来源：http://czr.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nst.epnwcf.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tyy.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://gci.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://htk.yanxiufei.cn

[I08] 贪婪与非贪婪匹配
来源：http://aat.birdmap.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tys.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://swk.0kj1m.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wee.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fcs.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dzs.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://chn.cashguo.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vem.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bxe.tian-w.cn

================================================================================
来源：http://elg.shanyushiyangtech.top

J. 日期与时间
来源：http://mcp.zdbjq.cn

================================================================================
来源：http://cli.yuanzhike.top

[J01] 获取当前时间
来源：http://sne.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uti.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mjr.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://eho.meibo888.top

TS:   new Date();  Date.now()
来源：http://nuo.ydzc1.top

Java: LocalDateTime.now();  Instant.now()
来源：http://njc.vehdjk.com

Go:   time.Now()
来源：http://whx.ywan-chungtsiang.top

Ruby: Time.now
来源：http://zca.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bkv.jinqigfzy.top

[J02] 格式化输出
来源：http://iib.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ora.gzhubu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oiq.ctjpmb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gbo.hesvh.cn

TS:   d.toISOString()
来源：http://rbk.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zex.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ogu.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rqm.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fzg.jyoumei.cn

[J03] 字符串解析为日期
来源：http://qcq.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dgy.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zlg.ivvv.top

JS:   new Date("2024-01-02")
来源：http://qbg.dashuyun.cn

TS:   new Date("2024-01-02")
来源：http://qxo.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://boz.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lrs.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://gjn.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://goj.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://vwj.cashguo.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ekw.shzxlz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wry.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ixn.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://igm.jinyuanbaomall.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nmy.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fns.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://abx.hammf.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://veh.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://ric.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://mkj.iojbl.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vmy.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wbm.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gxn.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://lsi.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://axl.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://mfc.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://bol.yonumen.top

[J06] 计算两时间之差
来源：http://dcx.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://ywo.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://ixy.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bce.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dmc.zhoulong.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://rne.tarul.cn

Go:   end.Sub(start).Hours()
来源：http://gfx.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://dcc.0kj1m.cn

C#:   (end - start).TotalSeconds
来源：http://nnw.zdbjq.cn

[J07] 比较两个日期
来源：http://ggi.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://uzu.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://czh.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kli.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://yfq.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ipe.jinqigfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ucj.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://sql.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://ioe.guowangkeji.top

[J08] 提取年月日与星期
来源：http://cuu.uphjek.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ila.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://atn.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qxr.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mux.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lvw.hysaishi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zfu.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://avb.ivvv.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rju.zhoulong.xyz

[J09] 时区处理
来源：http://alf.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vzp.gzhubu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vnj.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kjg.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uzp.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bal.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://njf.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://otc.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ybv.yanxiufei.cn

[J10] 取今天 / 本月第一天
来源：http://fel.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://umf.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vep.ybcxt.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aha.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pts.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blq.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://stk.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sjf.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uku.tanke756.top

================================================================================
来源：http://sal.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://bti.yvedp.cn

================================================================================
来源：http://bvs.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://coo.yanxiufei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ywc.yangfankeji.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kfi.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://ozj.cucudq.cn

TS:   JSON.stringify(obj)
来源：http://tzt.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://urh.bjfxy.top

Go:   json.Marshal(obj)
来源：http://tms.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xuv.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jyx.ctjpmb.com

[K02] JSON 字符串转对象
来源：http://ujw.cdnleiting.top

Py:   json.loads(s)
来源：http://fzu.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://adf.xinyue.icu

JS:   JSON.parse(s)
来源：http://mvv.shzxlz.cn

TS:   JSON.parse(s)
来源：http://wls.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tux.andypj.xyz

Go:   json.Unmarshal(data, &v)
来源：http://yln.yanxiufei.cn

Ruby: JSON.parse(s)
来源：http://xbx.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://giu.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://alo.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hyi.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ebw.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wlt.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lcr.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tyj.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jec.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://aqq.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nor.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://pie.daria6918.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ioj.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dja.jyoumei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sos.andypj.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ctq.yanxiufei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iww.9152youxi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nrl.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yzl.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kwt.yanxiufei.cn

[K05] 深拷贝对象
来源：http://nqx.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://wdp.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://hnu.smart0.xyz

JS:   structuredClone(obj)
来源：http://bnc.jyoumei.cn

TS:   structuredClone(obj)
来源：http://kko.yj202588.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lhi.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gez.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://syl.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mrc.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://pkr.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pfu.kuanghao11.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ofz.tian-w.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://imx.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tcm.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wbw.cheryme.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gut.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nkq.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ifg.chenzaomai.com

[K07] 进制转换
来源：http://cgc.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ewh.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jlu.jinqigfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ikn.hammf.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baa.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://keu.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ipa.bjfxy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kwx.shangyingyoupin.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://may.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://ljv.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://aem.jinghuilouyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ndz.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://jku.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://dmf.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jqz.aizwys.cn

Go:   encoding/gob
来源：http://gbj.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://kwy.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rsy.havefunace.top

================================================================================
来源：http://csy.fehbvm.com

L. 网络请求
来源：http://tej.sxryk.cn

================================================================================
来源：http://qwf.sxryk.cn

[L01] 发送 GET 请求
来源：http://syt.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gny.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eau.cucudq.cn

JS:   await fetch(url)
来源：http://new.xinyue.icu

TS:   await fetch(url)
来源：http://udf.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qlf.svipenyu.cn

Go:   resp, err := http.Get(url)
来源：http://qdk.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://pxj.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hyy.xuanzx.com

[L02] 发送 POST JSON
来源：http://pms.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://zyo.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zse.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tde.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mdb.yongpay.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gqt.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ahj.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rxh.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fle.vehdjk.com

[L03] 设置自定义请求头
来源：http://igy.hywenlv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://due.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vul.shanyushiyangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://azw.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xyq.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nzu.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wjg.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xdf.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cjx.iojbl.cn

[L04] 设置超时
来源：http://vqb.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://her.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cby.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dzi.dianchejie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wsr.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://crj.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://usr.meibo888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qnn.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sbr.smart0.xyz

[L05] 上传文件（multipart）
来源：http://cjp.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://egw.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hyt.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kwj.xylfe.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://avb.hnxiangtu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lar.birdmap.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zkd.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qir.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oau.xinyue.icu

[L06] 解析响应为 JSON
来源：http://plg.hfpthk.cn

Py:   resp.json()
来源：http://zct.cashguo.top

PHP:  json_decode($body, true);
来源：http://juu.yonumen.top

JS:   await resp.json()
来源：http://uap.bjfxy.top

TS:   await resp.json()
来源：http://dtd.dashuyun.cn


<!-- 参考信息 -->