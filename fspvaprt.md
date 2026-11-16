代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cfj.fzhhl.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lce.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qti.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pns.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mcd.hongshengwenyu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nuq.jqgufenzy.top

[I04] 正则替换
来源：http://fzw.pengpengdd.cyou

Py:   re.sub(r"\d+", "#", s)
来源：http://ssm.shzxlz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hdo.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mjo.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://cxx.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://bfu.tarul.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oue.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://enp.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mhx.zdbjq.cn

[I05] 按正则拆分
来源：http://heq.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yhr.bjfxy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ekj.jlsjyb.cn

JS:   s.split(/\s*,\s*/)
来源：http://qye.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://pvd.fanxiaobao.xyz

Java: s.split("\\s*,\\s*")
来源：http://zzi.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yfe.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://wba.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gud.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dtb.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://omj.tarul.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ifm.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xqf.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mxd.aizwys.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wxo.cqqwz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kvn.ctjpmb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dqv.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bow.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://jwg.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hut.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://njh.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lal.hongshengwenyu.top

TS:   /error/gim
来源：http://pdi.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lyt.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bfi.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://wes.xziqi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pcu.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://xbf.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://llu.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uul.ehwqpu.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sho.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pix.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hyf.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nxb.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ilz.kuanghao11.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ldt.chenlongwang.top

================================================================================
来源：http://xrb.uphjek.com

J. 日期与时间
来源：http://pij.bbcook.cn

================================================================================
来源：http://ybz.cashguo.top

[J01] 获取当前时间
来源：http://uei.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fvz.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wzt.yonumen.top

JS:   new Date();  Date.now()
来源：http://exr.jinyuanbaomall.cn

TS:   new Date();  Date.now()
来源：http://ccp.316326.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://wdw.kuanghao11.cn

Go:   time.Now()
来源：http://uht.xylfe.cn

Ruby: Time.now
来源：http://iiz.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nit.ivvv.top

[J02] 格式化输出
来源：http://osi.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://azw.sxryk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://svq.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xqm.zycfv.cn

TS:   d.toISOString()
来源：http://sxj.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yrr.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://btd.yj20258.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pms.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nex.hammf.cn

[J03] 字符串解析为日期
来源：http://xxy.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://duc.zhaomingkeji.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://erp.zhoulong.xyz

JS:   new Date("2024-01-02")
来源：http://ivl.nanxuanxn.top

TS:   new Date("2024-01-02")
来源：http://aeh.yj202588.top

Java: LocalDate.parse("2024-01-02")
来源：http://kqy.sjlbkw.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://obn.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://olg.yj20258888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qpb.jianghu66.top

[J04] 时间戳与日期互转
来源：http://gmi.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mbn.gzhubu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xfc.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://giv.hongshengwenyu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dfy.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dkw.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cqa.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pbw.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lvm.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://ybj.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://gug.chenjidiqi.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://lum.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kmi.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lvn.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://ziu.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cit.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://qbx.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://odr.ppjwa.cn

[J06] 计算两时间之差
来源：http://lrm.xingfuxueyuan.xyz

Py:   (end - start).total_seconds()
来源：http://lnq.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://gvt.nwbrower.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://woo.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ope.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gqp.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://wfr.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://vnj.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://dvq.yj20258.top

[J07] 比较两个日期
来源：http://xnh.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://mxj.c1oappe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oeq.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://tiv.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xmk.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xmy.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bum.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zao.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://pzf.zhaomingkeji.xyz

[J08] 提取年月日与星期
来源：http://uai.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pax.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kzv.pycfn.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zux.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rjm.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lwy.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nch.jinqigufen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lna.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zrf.jqgufenzy.top

[J09] 时区处理
来源：http://rrq.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iun.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vgf.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rpt.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://upj.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hgw.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lpc.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xmn.ybcxt.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xxv.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://svd.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yll.hywenlv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fgm.shanyushiyangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hbi.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ihz.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://chv.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xqm.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pvx.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iao.chenzaomai.com

================================================================================
来源：http://luw.kuanghao11.cn

K. JSON 与序列化
来源：http://yyx.hysaishi.cn

================================================================================
来源：http://fow.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://peh.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fex.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qdr.sweek.top

JS:   JSON.stringify(obj)
来源：http://keq.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://egc.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://phk.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://qlg.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://nzf.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nyy.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://bmr.ppjwa.cn

Py:   json.loads(s)
来源：http://ojo.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ikv.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://suj.sweek.top

TS:   JSON.parse(s)
来源：http://msh.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xir.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://wwa.yj20258.top

Ruby: JSON.parse(s)
来源：http://cwm.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gcv.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://jaq.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bjf.sjlbkw.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://axr.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://esx.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://dpl.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hpx.ivvv.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aem.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://dhw.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zje.nwbrower.top

[K04] 读取 JSON 文件
来源：http://wmn.iojbl.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xux.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sqk.pycfn.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dhm.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jyt.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kgw.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oer.kuanghao11.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kfr.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ubr.haohaochexian.top

[K05] 深拷贝对象
来源：http://bvr.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://vcw.52xcode.cn

PHP:  unserialize(serialize($obj));
来源：http://xej.ctjpmb.com

JS:   structuredClone(obj)
来源：http://uhq.xylfe.cn

TS:   structuredClone(obj)
来源：http://ovx.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xrw.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kbv.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wla.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rfh.ydzc1.top

[K06] 解析 URL 查询串
来源：http://jek.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iqo.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lki.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iki.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ggi.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fua.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rkf.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ppj.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nsh.ydzc1.top

[K07] 进制转换
来源：http://hud.snrcjt.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vkv.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mmb.0kj1m.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rsb.daxiang520.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rsp.chenjidiqi.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aui.cucudq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eno.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mic.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xhc.shanyushiyangtech.top

[K08] 二进制序列化（非 JSON）
来源：http://uyh.yongpay.top

Py:   pickle.dumps(obj)
来源：http://ivd.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jsz.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://unu.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://ttw.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://irt.hnxiangtu.top

Go:   encoding/gob
来源：http://loe.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://nbm.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dkv.uphjek.com

================================================================================
来源：http://qch.yueranfly.top

L. 网络请求
来源：http://wdc.yfazqb.com

================================================================================
来源：http://ahm.cqqwz.cn

[L01] 发送 GET 请求
来源：http://ayr.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sxg.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jfc.gotoacloud.top

JS:   await fetch(url)
来源：http://kxt.ivvv.top

TS:   await fetch(url)
来源：http://eoz.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ygy.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://uvb.shangyingyoupin.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iqu.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qlh.yanxiufei.cn

[L02] 发送 POST JSON
来源：http://niv.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://qky.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rsm.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vlg.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rnc.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sga.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tvt.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zlx.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eun.sysykeji.top

[L03] 设置自定义请求头
来源：http://aue.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bdc.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gtg.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sbb.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xyu.sweek.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nbu.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gmw.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ahy.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wvh.tarul.cn

[L04] 设置超时
来源：http://tyg.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://hnq.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://utj.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fro.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ygc.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yzw.zhixingplan.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eoc.shzxlz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://svq.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lxh.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://rrm.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gsj.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://onx.smart0.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://doz.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ocw.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jlz.tarul.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qla.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cve.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://opv.vehdjk.com

[L06] 解析响应为 JSON
来源：http://bss.zhaomingkeji.xyz

Py:   resp.json()
来源：http://vnu.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://ayi.hongshengwenyu.top

JS:   await resp.json()
来源：http://mlz.hongshengwenyu.top

TS:   await resp.json()
来源：http://joq.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tfz.gaohongyu789.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hyn.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://fds.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://urr.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://fkl.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eev.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ipa.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://cvr.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://pzr.quarkkingdee.top

Java: resp.statusCode()
来源：http://nkh.jqgfzy.top

Go:   resp.StatusCode
来源：http://fpr.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://mgd.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://yjg.iojbl.cn

[L08] 并发请求多个地址
来源：http://hln.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vws.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://zcr.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://doz.zhijiandao.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gnc.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://svx.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rig.yuxming.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://btr.yongpay.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jpc.ydzc1.top

================================================================================
来源：http://pso.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://yye.ppjwa.cn

================================================================================
来源：http://bpj.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://zdj.daxiang520.top

Py:   sys.argv[1:]
来源：http://gbi.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://heh.ppjwa.cn


<!-- 参考信息 -->