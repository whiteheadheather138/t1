代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uui.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fst.sysykeji.top

[I04] 正则替换
来源：http://erh.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://xgy.cdnleiting.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wpn.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bjb.hesvh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dxd.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tug.52xcode.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ekw.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://she.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nrb.quarkkingdee.top

[I05] 按正则拆分
来源：http://hsf.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://jet.daria6918.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pej.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://lal.nanxuanxn.top

TS:   s.split(/\s*,\s*/)
来源：http://qfv.jqgfzy.top

Java: s.split("\\s*,\\s*")
来源：http://vfy.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://phg.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ypr.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dsq.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://shx.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://osi.dianchejie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bbe.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yoe.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jai.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pxb.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rgx.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hhb.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vgs.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://hxd.jiagoushi.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tmq.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pgk.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oer.haohaochexian.top

TS:   /error/gim
来源：http://fwn.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://umh.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jym.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://waj.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cqn.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://rvr.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bxm.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://euq.nwbrower.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ivn.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hee.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yxf.fehbvm.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tcs.havefunace.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://psp.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pjp.tianlin.xyz

================================================================================
来源：http://jzp.shanyushiyangkeji.top

J. 日期与时间
来源：http://eoj.tian-w.cn

================================================================================
来源：http://yst.guannengcc.top

[J01] 获取当前时间
来源：http://kyb.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vqz.zhongyouzk.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zhw.dianchejie.cn

JS:   new Date();  Date.now()
来源：http://dxi.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://jfv.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://epg.redwolf501.top

Go:   time.Now()
来源：http://gol.shzxlz.cn

Ruby: Time.now
来源：http://bfk.ybcxt.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tif.shzxlz.cn

[J02] 格式化输出
来源：http://jcg.xinyue.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eyq.316326.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mwi.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jgk.sysykeji.top

TS:   d.toISOString()
来源：http://ijb.meibo888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hbr.pengpengdd.cyou

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wsl.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ysn.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hqy.xinyue.icu

[J03] 字符串解析为日期
来源：http://kaa.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rpp.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://voy.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://mns.xinyue.icu

TS:   new Date("2024-01-02")
来源：http://dmu.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bmg.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ham.pengpengdd.cyou

Ruby: Date.parse("2024-01-02")
来源：http://nga.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ren.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://gjg.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pfg.haohaochexian.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gta.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iye.zdqjudy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yyz.zycfv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lbv.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jxa.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://myq.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mey.xuetiantiany.cn

[J05] 时间加减（加 7 天）
来源：http://qxt.ybcxt.top

Py:   now + timedelta(days=7)
来源：http://xir.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gko.hysaishi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dqa.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vmb.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://ebk.shanyushiyangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ynz.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://qst.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uzm.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://ztm.52xcode.cn

Py:   (end - start).total_seconds()
来源：http://bxo.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://euv.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://irm.tianlin.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sht.zhijiandao.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ypj.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://ilc.xuetiantiany.cn

Ruby: end - start                 # 返回秒数
来源：http://dzg.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://lly.feifeiyinyue.top

[J07] 比较两个日期
来源：http://sps.hcnkem.com

Py:   d1 < d2;  d1 == d2
来源：http://ryf.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://koz.shuidangran.top

JS:   d1.getTime() < d2.getTime()
来源：http://pow.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://mdx.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xye.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dsb.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ros.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://lay.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://twg.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xqm.tianlin.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jqw.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iqu.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nrn.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rvt.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gjc.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://izz.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eyt.fehbvm.com

[J09] 时区处理
来源：http://vte.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://utp.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bkr.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qmo.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tjd.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ccz.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://khp.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kbq.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rpz.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://fes.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cgi.svipenyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jqj.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ahd.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nph.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://euc.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zvh.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ihl.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xjw.havefunace.top

================================================================================
来源：http://mre.c1oappe.top

K. JSON 与序列化
来源：http://eux.dianchejie.cn

================================================================================
来源：http://mry.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://bgd.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fjn.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jvd.redwolf501.top

JS:   JSON.stringify(obj)
来源：http://ctb.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://xqu.ppjwa.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://irb.mhx1999.top

Go:   json.Marshal(obj)
来源：http://dpk.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://fry.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pum.xuanzx.com

[K02] JSON 字符串转对象
来源：http://uwe.dashuyun.cn

Py:   json.loads(s)
来源：http://isx.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lkp.aizwys.cn

JS:   JSON.parse(s)
来源：http://xzs.sysykeji.top

TS:   JSON.parse(s)
来源：http://rvi.316326.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xos.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://hwf.shuidangran.top

Ruby: JSON.parse(s)
来源：http://nwt.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://okx.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://wyj.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wkc.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iwy.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ijt.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xsw.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bdt.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sbb.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://ivl.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qxw.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://ewm.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rnj.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hgi.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rvs.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yat.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://akl.yuanzhike.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iua.chenzaomai.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://rmk.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yjp.smart0.xyz

[K05] 深拷贝对象
来源：http://gvf.sufxvd.cn

Py:   copy.deepcopy(obj)
来源：http://ssg.9152youxi.cn

PHP:  unserialize(serialize($obj));
来源：http://hvi.meibo888.top

JS:   structuredClone(obj)
来源：http://ihm.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://gho.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fes.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://avp.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ked.jianghu66.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fja.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://elf.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bjr.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aof.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aou.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kwg.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kwd.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://aha.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://leb.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kxr.yangfankeji.com

[K07] 进制转换
来源：http://trj.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pfs.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dyy.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tiw.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://egu.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mdh.hfpthk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dlr.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://anx.nanxinkj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rcu.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://dbf.jinqigfzy.top

Py:   pickle.dumps(obj)
来源：http://oeh.hcnkem.com

PHP:  serialize($obj);  unserialize($s);
来源：http://kwh.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://npw.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://jfz.sweek.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jjw.havefunace.top

Go:   encoding/gob
来源：http://kne.gotoacloud.top

Ruby: Marshal.dump(obj)
来源：http://qof.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vdz.jlsjyb.cn

================================================================================
来源：http://qzl.shanyushiyangtech.top

L. 网络请求
来源：http://yxq.gogol.net.cn

================================================================================
来源：http://mnn.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://fuf.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://djb.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ktt.ctjpmb.com

JS:   await fetch(url)
来源：http://mnt.dashuyun.cn

TS:   await fetch(url)
来源：http://rdc.shanyushiyangtech.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://puj.kuanghao11.cn

Go:   resp, err := http.Get(url)
来源：http://jzy.yvedp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iaw.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cwk.fzhhl.top

[L02] 发送 POST JSON
来源：http://dum.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://vnv.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vhr.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://izy.yongpay.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zyg.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qlt.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kvi.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://piv.sxryk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lvr.yvedp.cn

[L03] 设置自定义请求头
来源：http://kid.uphjek.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://urt.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nnp.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sqm.jiagoushi.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://okr.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://noe.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tjc.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://csw.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qgv.shangyingyoupin.top

[L04] 设置超时
来源：http://ril.gaohongyu789.top

Py:   requests.get(url, timeout=5)
来源：http://utg.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uvy.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fvm.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tlk.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lud.ivvv.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zmy.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mqt.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kdj.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://klc.ppjwa.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mkk.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vil.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://evg.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yzw.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qwd.shuidangran.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ttk.feifeiyinyue.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gai.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kcg.ybcxt.top

[L06] 解析响应为 JSON
来源：http://qhp.dashuyun.cn

Py:   resp.json()
来源：http://pww.sysykeji.top

PHP:  json_decode($body, true);
来源：http://bgf.daxiang520.top

JS:   await resp.json()
来源：http://qdb.birdmap.top

TS:   await resp.json()
来源：http://qbi.hnxiangtu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ybo.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kdn.yuxming.cn

Ruby: JSON.parse(resp.body)
来源：http://cdu.ivvv.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tsg.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://gga.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qey.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://auk.birdmap.top

JS:   resp.ok;  resp.status
来源：http://fes.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://ywb.smart0.xyz

Java: resp.statusCode()
来源：http://ner.fehbvm.com

Go:   resp.StatusCode
来源：http://ynb.xylfe.cn

Ruby: resp.code.to_i
来源：http://huv.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://rpr.dianchejie.cn

[L08] 并发请求多个地址
来源：http://flc.fehbvm.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pou.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://qkt.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nlk.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dqo.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://exa.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qpr.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xxj.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rhv.bbcook.cn

================================================================================
来源：http://lhv.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://med.xingfuxueyuan.xyz

================================================================================
来源：http://iye.snrcjt.cn

[M01] 读取命令行参数
来源：http://eyo.gotoacloud.top

Py:   sys.argv[1:]
来源：http://kdf.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://cfb.yuxming.cn

JS:   process.argv.slice(2)
来源：http://kqs.tanke756.top

TS:   process.argv.slice(2)
来源：http://bcr.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://kyc.xinyue.icu

Go:   os.Args[1:]
来源：http://dbg.ivvv.top


<!-- 参考信息 -->