代发 wailian999

TS:   s.match(/\d+/g)
来源：http://dhw.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pqe.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wda.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://roj.xuetiantiany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bgw.hesvh.cn

[I03] 提取捕获分组
来源：http://gwn.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://key.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fei.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oiq.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pre.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oqq.hnxiangtu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rin.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dos.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xag.fktsv.cn

[I04] 正则替换
来源：http://zve.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ibo.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ffc.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kzg.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://kdj.yfazqb.com

Java: s.replaceAll("\\d+", "#")
来源：http://oyo.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jzb.zhaomingkeji.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://zbm.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fog.jqgfzy.top

[I05] 按正则拆分
来源：http://mkt.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bxm.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pjj.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://uwo.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://yxw.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://rsk.316326.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zpn.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://zyl.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://etx.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fto.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cwx.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wol.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://may.yj20258.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://opi.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gqd.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ove.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wxn.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://idx.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://eqo.gzhubu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rao.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ris.nanxinkj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hra.jinqigfzy.top

TS:   /error/gim
来源：http://ltx.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://slf.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://abg.chenlongwang.top

Ruby: s.scan(/error/i)
来源：http://xlk.jinyuanbaomall.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ryp.jyoumei.cn

[I08] 贪婪与非贪婪匹配
来源：http://kiu.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oea.snrcjt.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lby.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xlb.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jux.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jkw.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bkz.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jnb.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://smu.ydjk.org.cn

================================================================================
来源：http://lzh.jyoumei.cn

J. 日期与时间
来源：http://max.yanxiufei.cn

================================================================================
来源：http://xzs.wangdashe.top

[J01] 获取当前时间
来源：http://nqc.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nji.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ctx.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://xhm.gzhubu.top

TS:   new Date();  Date.now()
来源：http://yaa.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://yta.zhiwuduotai.top

Go:   time.Now()
来源：http://psc.pengpengdd.cyou

Ruby: Time.now
来源：http://fxq.yangfankeji.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lsd.fengsongda.top

[J02] 格式化输出
来源：http://vth.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kra.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gty.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jji.shangyingyoupin.top

TS:   d.toISOString()
来源：http://mza.gotoacloud.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xup.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nbz.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zjp.316326.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zss.redwolf501.top

[J03] 字符串解析为日期
来源：http://wxz.yuxming.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yuk.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vxi.tianlin.xyz

JS:   new Date("2024-01-02")
来源：http://ljc.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://sqo.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jkw.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tnv.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://dex.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zpi.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://sjf.ctjpmb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lcp.pengpengdd.cyou

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pmw.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mcj.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://rlz.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hpa.sjlbkw.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://drq.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qcb.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ubv.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://ggh.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://utu.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://pfm.mhx1999.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kiq.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kvw.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://wyi.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pzb.yongpay.top

Ruby: Time.now + 7 * 86400
来源：http://kcn.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://xbe.jyoumei.cn

[J06] 计算两时间之差
来源：http://ceq.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://gkj.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://xez.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wjj.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://flw.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://lgi.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://eqv.yvedp.cn

Ruby: end - start                 # 返回秒数
来源：http://vnl.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://rxj.jqgufenzy.top

[J07] 比较两个日期
来源：http://dqq.ctjpmb.com

Py:   d1 < d2;  d1 == d2
来源：http://xzt.0kj1m.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pox.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://crn.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://pua.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://atf.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://szk.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://aeo.zycfv.cn

C#:   d1 < d2;  d1 == d2
来源：http://dir.shzxlz.cn

[J08] 提取年月日与星期
来源：http://dky.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kkb.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gai.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bxh.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ede.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oiq.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://edb.ydjk.org.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fsd.zhijiandao.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mqj.316326.xyz

[J09] 时区处理
来源：http://aax.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oxd.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jac.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yiv.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nql.cashguo.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tyl.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kfp.jianghu66.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yjv.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nuv.yanxiufei.cn

[J10] 取今天 / 本月第一天
来源：http://kok.ctjpmb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://gkq.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xcv.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iah.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dct.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dtk.jqgufenzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://owa.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://amb.sweek.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nnc.gaohongyu789.top

================================================================================
来源：http://lcn.yvedp.cn

K. JSON 与序列化
来源：http://cty.zhiwuduotai.top

================================================================================
来源：http://dpf.dianchejie.cn

[K01] 对象转 JSON 字符串
来源：http://hpf.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nhe.jinqigfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wln.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://eah.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://tuh.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bgw.ppjwa.cn

Go:   json.Marshal(obj)
来源：http://mqe.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://nks.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hyk.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://yre.bbcook.cn

Py:   json.loads(s)
来源：http://kkw.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://boa.9152youxi.cn

JS:   JSON.parse(s)
来源：http://eum.zycfv.cn

TS:   JSON.parse(s)
来源：http://lwu.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://scs.xinyue.icu

Go:   json.Unmarshal(data, &v)
来源：http://mbi.yj202588.top

Ruby: JSON.parse(s)
来源：http://uid.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://axf.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://qee.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aoh.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cua.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://dsq.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lzb.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jyl.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gci.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tmg.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xza.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://evu.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vys.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dcl.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uxw.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lmn.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yrb.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ahj.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://phe.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ilx.9152youxi.cn

[K05] 深拷贝对象
来源：http://odm.epnwcf.com

Py:   copy.deepcopy(obj)
来源：http://hbj.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://qor.jqgfzy.top

JS:   structuredClone(obj)
来源：http://bce.havefunace.top

TS:   structuredClone(obj)
来源：http://lqb.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sry.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pzq.wangshuangyany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xpn.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wwl.wangdashe.top

[K06] 解析 URL 查询串
来源：http://jhg.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dfn.ctjpmb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tfi.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vnf.shuidangran.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://edn.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vvy.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ckl.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://znp.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://koz.kuanghao11.cn

[K07] 进制转换
来源：http://jyb.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gig.hnqzz.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://twh.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gto.shangyingyoupin.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pmv.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xdl.yanxiufei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mhe.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://flk.yvedp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://inz.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://nbh.epnwcf.com

Py:   pickle.dumps(obj)
来源：http://vwu.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rol.zdqjudy.top

JS:   v8.serialize(obj)        // Node
来源：http://uuh.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://fpi.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jxv.c1oappe.top

Go:   encoding/gob
来源：http://fww.yongpay.top

Ruby: Marshal.dump(obj)
来源：http://gdd.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://erx.bjfxy.top

================================================================================
来源：http://mzj.zhengqikj.top

L. 网络请求
来源：http://oyj.jyoumei.cn

================================================================================
来源：http://elz.jianghu66.top

[L01] 发送 GET 请求
来源：http://vpm.chenjidiqi.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fdv.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bgk.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://yqu.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://uah.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rea.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://bop.fanxiaobao.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://wgk.zhijiandao.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lvp.gzhubu.top

[L02] 发送 POST JSON
来源：http://qli.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://ien.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tvd.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hdn.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zqn.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kwu.dianchejie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ezs.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qhe.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xyh.ivvv.top

[L03] 设置自定义请求头
来源：http://peh.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xin.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fgm.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hez.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ttq.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pyi.yj20258.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hrg.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ich.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ljo.hywenlv.cn

[L04] 设置超时
来源：http://uvd.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://xik.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bzp.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nit.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nqp.nanxuanxn.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kuk.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://llk.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tlf.smart0.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://niu.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://haf.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://huh.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://crz.gaohongyu789.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qqh.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ytz.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oqx.svipenyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ygb.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ttg.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lih.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://bpt.guowangkeji.top

Py:   resp.json()
来源：http://syx.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://atq.xuanzx.com

JS:   await resp.json()
来源：http://yrz.andypj.xyz

TS:   await resp.json()
来源：http://ztu.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vtr.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eag.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://vxj.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wln.aizwys.cn

[L07] 处理 HTTP 状态码
来源：http://mjh.sysykeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hlw.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nmq.hammf.cn

JS:   resp.ok;  resp.status
来源：http://gah.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://lrm.feifeiyinyue.top

Java: resp.statusCode()
来源：http://kyz.jqgfzy.top

Go:   resp.StatusCode
来源：http://iyv.hfpthk.cn

Ruby: resp.code.to_i
来源：http://qhh.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://jtp.chenzaomai.com

[L08] 并发请求多个地址
来源：http://aqj.epnwcf.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dwk.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://dwt.xuetiantiany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gvi.zhongyouzk.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iua.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://brw.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xki.chenjidiqi.icu


<!-- 参考信息 -->