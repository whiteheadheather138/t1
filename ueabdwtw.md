代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eub.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hhr.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sme.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mra.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mmy.hongshengwenyu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wrc.sweek.top

[I04] 正则替换
来源：http://paf.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bau.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ypg.ehwqpu.com

JS:   s.replace(/\d+/g, "#")
来源：http://wwy.shanyushiyangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://glc.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://cug.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ihf.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wxz.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eey.fehbvm.com

[I05] 按正则拆分
来源：http://wuw.vqdsnc.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://byr.pengpengdd.cyou

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mby.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://tgz.zdqjudy.top

TS:   s.split(/\s*,\s*/)
来源：http://tga.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://flx.cashguo.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wsz.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dde.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hct.xinyue.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zwv.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://adg.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wbq.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://khi.svipenyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lqx.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mbw.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sfp.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pel.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://elq.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://zma.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nph.xuanzx.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hjp.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qav.yuanzhike.top

TS:   /error/gim
来源：http://ofy.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ccj.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://suh.tanke756.top

Ruby: s.scan(/error/i)
来源：http://cba.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pti.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://hdc.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kyi.daria6918.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lqy.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kzo.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rbs.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tlp.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yqi.hywenlv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zud.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sws.nanxuanxn.top

================================================================================
来源：http://gqe.shanyushiyangkeji.top

J. 日期与时间
来源：http://ilr.bjfxy.top

================================================================================
来源：http://zwb.cashguo.top

[J01] 获取当前时间
来源：http://xsv.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ziq.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dec.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://gvh.sufxvd.cn

TS:   new Date();  Date.now()
来源：http://ioc.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dpc.feifeiyinyue.top

Go:   time.Now()
来源：http://mih.hnxiangtu.top

Ruby: Time.now
来源：http://lvs.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pye.hesvh.cn

[J02] 格式化输出
来源：http://zuz.jqgufenzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lqa.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jvd.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ytj.0kj1m.cn

TS:   d.toISOString()
来源：http://duz.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iyf.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ivz.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xsw.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hge.gotoacloud.top

[J03] 字符串解析为日期
来源：http://wjf.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hqd.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sio.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://blm.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://rnc.aizwys.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eiy.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zzi.jiagoushi.top

Ruby: Date.parse("2024-01-02")
来源：http://zas.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zwt.yonumen.top

[J04] 时间戳与日期互转
来源：http://gnv.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xuf.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ltu.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bbi.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://hqu.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tep.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ktn.tanke756.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://frt.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zoq.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://kku.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://qsm.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://wzr.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://krq.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ulr.daria6918.cn

Java: LocalDate.now().plusDays(7)
来源：http://xxa.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rqe.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://kwj.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://dri.hfpthk.cn

[J06] 计算两时间之差
来源：http://pdb.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://sbv.zhixingplan.top

PHP:  $end->diff($start)->days;
来源：http://for.aibaodan.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rer.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kuo.nanxinkj.top

Java: Duration.between(start, end).toSeconds()
来源：http://ame.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://dnu.guowangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://kdt.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://wit.yueranfly.top

[J07] 比较两个日期
来源：http://hud.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://jlj.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dys.wangshuangyany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bpy.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://kdz.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qti.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hcp.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://ero.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://dzy.yueranfly.top

[J08] 提取年月日与星期
来源：http://cpx.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pzx.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nmq.hywenlv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hpo.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xkr.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dpn.havefunace.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nss.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hlo.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gam.dianchejie.cn

[J09] 时区处理
来源：http://fck.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ybm.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xjj.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://spl.vehdjk.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qxc.jinqigufen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gfy.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sgh.xuanzx.com

Ruby: Time.now.getlocal("+08:00")
来源：http://nwi.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fdn.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://fca.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://eoi.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qfi.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kgr.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lhq.hesvh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hzu.cucudq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oyi.jianghu66.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kwj.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://unw.xziqi.cn

================================================================================
来源：http://dwd.andypj.xyz

K. JSON 与序列化
来源：http://ugd.iojbl.cn

================================================================================
来源：http://qmf.xingfuxueyuan.xyz

[K01] 对象转 JSON 字符串
来源：http://gep.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lbc.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uzo.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://azf.cheryme.top

TS:   JSON.stringify(obj)
来源：http://whg.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dbg.tanke756.top

Go:   json.Marshal(obj)
来源：http://bzf.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://kla.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ytg.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://vxf.nanxuanxn.top

Py:   json.loads(s)
来源：http://hcl.nanxinkj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fnj.cucudq.cn

JS:   JSON.parse(s)
来源：http://vyi.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://nao.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://civ.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://sbz.epnwcf.com

Ruby: JSON.parse(s)
来源：http://bpi.meibo888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oah.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://opo.yonumen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fnq.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ygu.aibaodan.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pad.guowangkeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fjr.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wjj.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://caw.hongshengwenyu.top

Ruby: JSON.pretty_generate(obj)
来源：http://coi.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cil.52xcode.cn

[K04] 读取 JSON 文件
来源：http://ehv.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xis.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://clc.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://odh.nanxuanxn.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cvi.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://grz.hcnkem.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fip.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fki.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ttc.sysykeji.top

[K05] 深拷贝对象
来源：http://qty.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://hrp.yongpay.top

PHP:  unserialize(serialize($obj));
来源：http://ult.havefunace.top

JS:   structuredClone(obj)
来源：http://wts.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://xbe.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mrd.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rsc.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ixx.dashuyun.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hci.fktsv.cn

[K06] 解析 URL 查询串
来源：http://skd.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pca.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vwk.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fdd.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gde.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uyt.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://deb.bbcook.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://boj.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lgl.shuidangran.top

[K07] 进制转换
来源：http://hpt.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://onj.yanxiufei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ymo.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xqa.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ley.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xeq.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://esh.hnxiangtu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nkh.zycfv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zom.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://dni.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://kaw.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mem.shanyushiyangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://kyt.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://oya.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qpn.smart0.xyz

Go:   encoding/gob
来源：http://sny.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://uls.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nkj.fengsongda.top

================================================================================
来源：http://qdj.jyoumei.cn

L. 网络请求
来源：http://mfg.iojbl.cn

================================================================================
来源：http://ulj.shuidangran.top

[L01] 发送 GET 请求
来源：http://utf.mhx1999.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://upg.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nsn.ehwqpu.com

JS:   await fetch(url)
来源：http://bzt.fktsv.cn

TS:   await fetch(url)
来源：http://gog.shanyushiyangtech.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wpr.shangyingyoupin.top

Go:   resp, err := http.Get(url)
来源：http://bsc.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://snk.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gge.tian-w.cn

[L02] 发送 POST JSON
来源：http://mdm.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://ahv.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bnm.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tjx.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pcr.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iqu.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qly.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://phl.gotoacloud.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://igy.ydjk.org.cn

[L03] 设置自定义请求头
来源：http://cgm.hnqzz.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xjc.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eat.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qen.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fzl.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zxu.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dss.redwolf501.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oaq.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xec.chenjidiqi.icu

[L04] 设置超时
来源：http://gek.hammf.cn

Py:   requests.get(url, timeout=5)
来源：http://opc.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://crm.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fca.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://equ.fanxiaobao.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xfr.redwolf501.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://goh.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cjq.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cpv.cucudq.cn

[L05] 上传文件（multipart）
来源：http://aqa.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ile.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://glq.jqgfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zkx.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hla.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bnc.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hgn.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uti.hongshengwenyu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://roy.fanxiaobao.xyz

[L06] 解析响应为 JSON
来源：http://fez.zhixingplan.top

Py:   resp.json()
来源：http://vgm.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://pcp.aibaodan.cn

JS:   await resp.json()
来源：http://tif.cqqwz.cn

TS:   await resp.json()
来源：http://pmw.hesvh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pqr.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eya.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://unj.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rfo.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://piw.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://raj.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yzl.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://hkh.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://qms.kuanghao11.cn

Java: resp.statusCode()
来源：http://guq.yfazqb.com

Go:   resp.StatusCode
来源：http://mky.shzxlz.cn

Ruby: resp.code.to_i
来源：http://jik.havefunace.top

C#:   (int)resp.StatusCode
来源：http://ivq.tianlin.xyz

[L08] 并发请求多个地址
来源：http://acj.daria6918.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tzl.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://oom.yj20258.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yfi.sjlbkw.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pvw.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ehl.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nqh.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kvl.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gqc.fengsongda.top

================================================================================
来源：http://kma.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://wup.feifeiyinyue.top

================================================================================
来源：http://qrt.aibaodan.cn

[M01] 读取命令行参数
来源：http://ffu.ivvv.top

Py:   sys.argv[1:]
来源：http://arn.yanxiufei.cn

PHP:  $argv;  $argc;
来源：http://qmj.jianghu66.top


<!-- 参考信息 -->