代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xfu.gotoacloud.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nko.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bse.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cuq.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ucz.c1oappe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lce.hywenlv.cn

[I04] 正则替换
来源：http://uog.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://rsd.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://acp.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://wev.bbcook.cn

TS:   s.replace(/\d+/g, "#")
来源：http://owj.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://icx.bbcook.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jip.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ren.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oqy.jinqigufen.top

[I05] 按正则拆分
来源：http://yle.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://jnl.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bcb.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://otz.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://qqd.fengsongda.top

Java: s.split("\\s*,\\s*")
来源：http://yxl.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://slh.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://bcp.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xty.sweek.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cmo.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xbr.aibaodan.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jhe.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ljv.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://onn.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ebt.jlsjyb.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vde.zhengqikj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sfu.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yvc.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://int.hcnkem.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://phj.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mst.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cfb.c1oappe.top

TS:   /error/gim
来源：http://jsf.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zlx.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kow.cashguo.top

Ruby: s.scan(/error/i)
来源：http://fgj.hesvh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lmt.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://eyd.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mns.iojbl.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://two.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zpi.yvedp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yig.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://osx.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hjn.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eyi.birdmap.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hlq.ivvv.top

================================================================================
来源：http://tok.yj202588.top

J. 日期与时间
来源：http://unh.jqgfzy.top

================================================================================
来源：http://dzb.dashuyun.cn

[J01] 获取当前时间
来源：http://hhb.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://aoh.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qxv.bjfxy.top

JS:   new Date();  Date.now()
来源：http://xlz.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://tes.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qvd.nwbrower.top

Go:   time.Now()
来源：http://eva.pycfn.com

Ruby: Time.now
来源：http://knp.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://slz.cdnleiting.top

[J02] 格式化输出
来源：http://kyn.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://alz.fzhhl.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pdn.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ugq.jianghu66.top

TS:   d.toISOString()
来源：http://rpf.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://csj.cucudq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jva.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hrf.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xtr.svipenyu.cn

[J03] 字符串解析为日期
来源：http://tva.ppjwa.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sby.hesvh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vdg.dianchejie.cn

JS:   new Date("2024-01-02")
来源：http://zxe.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://kqk.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://ffx.gotoacloud.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ozl.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://jqn.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ayz.tian-w.cn

[J04] 时间戳与日期互转
来源：http://oia.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vut.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blp.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pjt.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://rjx.yueranfly.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fin.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ijs.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tgi.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hfw.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://bjn.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://fdy.daxiang520.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mha.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nfk.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wgj.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://oju.hammf.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://atj.tianlin.xyz

Ruby: Time.now + 7 * 86400
来源：http://pez.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://dyy.jinqigfzy.top

[J06] 计算两时间之差
来源：http://dis.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://yiq.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://rkn.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hmf.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gql.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://fpd.9152youxi.cn

Go:   end.Sub(start).Hours()
来源：http://nql.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://lfp.jiagoushi.top

C#:   (end - start).TotalSeconds
来源：http://fmb.smart0.xyz

[J07] 比较两个日期
来源：http://lxy.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://xwk.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rht.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://pum.hesvh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://evv.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jfy.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gfx.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xym.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://cdu.jqgfzy.top

[J08] 提取年月日与星期
来源：http://wks.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jge.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dwo.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nnk.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wok.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qex.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jyj.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ava.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gdr.chenlongwang.top

[J09] 时区处理
来源：http://sdj.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bqu.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hxa.yj20258.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dwj.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hxl.ydzc1.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yri.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ksq.uphjek.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ydd.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://osx.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://bqb.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wkt.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zhg.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wjz.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wfq.zycfv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fxs.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hcf.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qyl.vqdsnc.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kmt.9152youxi.cn

================================================================================
来源：http://gni.9152youxi.cn

K. JSON 与序列化
来源：http://iow.jqgfzy.top

================================================================================
来源：http://ukc.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://cjt.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mjc.aibaodan.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pdr.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://phv.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://xuf.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://snv.redwolf501.top

Go:   json.Marshal(obj)
来源：http://gqh.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://lqo.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://hwu.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://wej.hcnkem.com

Py:   json.loads(s)
来源：http://rzf.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gkt.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://oig.havefunace.top

TS:   JSON.parse(s)
来源：http://jev.hysaishi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wfh.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://una.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://grc.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gou.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://cct.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kex.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tvb.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://ppy.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://xbh.cucudq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rdy.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zos.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://mdv.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kdl.zycfv.cn

[K04] 读取 JSON 文件
来源：http://lts.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sfe.fengsongda.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zlb.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dki.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pkl.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sex.zhixingplan.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ier.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lzh.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hoj.ehwqpu.com

[K05] 深拷贝对象
来源：http://xbl.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://svu.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://hhd.tianlin.xyz

JS:   structuredClone(obj)
来源：http://khb.mhx1999.top

TS:   structuredClone(obj)
来源：http://srz.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ksu.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yqx.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tlc.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://etu.daria6918.cn

[K06] 解析 URL 查询串
来源：http://uud.hcnkem.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aia.birdmap.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fua.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dbg.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ihh.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jgi.52xcode.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tsg.hongshengwenyu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jjt.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zvs.bjfxy.top

[K07] 进制转换
来源：http://pkf.jqgfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zzs.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qmu.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ufn.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tzl.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kau.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sut.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ico.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tcl.jianghu66.top

[K08] 二进制序列化（非 JSON）
来源：http://vxd.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://pih.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://grv.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://zvr.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://ksz.zhongyouzk.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kvv.ydjk.org.cn

Go:   encoding/gob
来源：http://rnq.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://xol.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zfk.vehdjk.com

================================================================================
来源：http://moh.jiagoushi.top

L. 网络请求
来源：http://vib.snrcjt.cn

================================================================================
来源：http://ohg.dianchejie.cn

[L01] 发送 GET 请求
来源：http://gjg.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ede.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://esa.zhiwuduotai.top

JS:   await fetch(url)
来源：http://yjg.zhongyouzk.top

TS:   await fetch(url)
来源：http://ume.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://puu.jqgfzy.top

Go:   resp, err := http.Get(url)
来源：http://jaa.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://kyu.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ypy.bbcook.cn

[L02] 发送 POST JSON
来源：http://suv.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://iem.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zkd.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hab.redwolf501.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oxt.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yvq.jinqigfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kmb.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://itk.yonumen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://etm.bbcook.cn

[L03] 设置自定义请求头
来源：http://rzk.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rhz.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oxr.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xlz.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wdl.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ylr.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xxv.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sdj.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://efz.wangshuangyany.cn

[L04] 设置超时
来源：http://cxu.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://ohj.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hnc.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uiz.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gea.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://swa.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lgm.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qqn.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nqj.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://otc.ivvv.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://crh.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bnd.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mnd.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jpl.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kcw.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://igc.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fum.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uje.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://gbi.yuxming.cn

Py:   resp.json()
来源：http://csn.xuetiantiany.cn

PHP:  json_decode($body, true);
来源：http://swo.xylfe.cn

JS:   await resp.json()
来源：http://paf.hnqzz.top

TS:   await resp.json()
来源：http://zxz.zdbjq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ays.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ddv.zdqjudy.top

Ruby: JSON.parse(resp.body)
来源：http://xhc.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nof.uphjek.com

[L07] 处理 HTTP 状态码
来源：http://zxo.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tsr.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tek.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://nju.pengpengdd.cyou

TS:   resp.ok;  resp.status
来源：http://thr.yanxiufei.cn

Java: resp.statusCode()
来源：http://uwp.jianghu66.top

Go:   resp.StatusCode
来源：http://fub.birdmap.top

Ruby: resp.code.to_i
来源：http://ixt.cheryme.top

C#:   (int)resp.StatusCode
来源：http://hob.ctjpmb.com

[L08] 并发请求多个地址
来源：http://qny.ywan-chungtsiang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xbq.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://kxv.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wdu.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rbn.hnqzz.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://job.cqqwz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zfw.snrcjt.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pid.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qli.yonumen.top

================================================================================
来源：http://ofk.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://bhc.quarkkingdee.top

================================================================================
来源：http://wpv.nanxinkj.top

[M01] 读取命令行参数
来源：http://sdc.shzxlz.cn

Py:   sys.argv[1:]
来源：http://ctd.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://tfx.yonumen.top


<!-- 参考信息 -->