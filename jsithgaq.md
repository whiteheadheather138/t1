代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://rkf.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://aoa.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xza.yj202588.top

[I05] 按正则拆分
来源：http://lhk.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://tbv.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nhb.chenzaomai.com

JS:   s.split(/\s*,\s*/)
来源：http://bqs.hfpthk.cn

TS:   s.split(/\s*,\s*/)
来源：http://gth.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://ouu.meibo888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wqj.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://sty.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hdx.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://miv.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://efy.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fdk.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uob.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hxt.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://riu.shzxlz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ict.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://brk.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lyq.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://mbp.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://szs.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vcm.hammf.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rop.jqgfzy.top

TS:   /error/gim
来源：http://tzl.shangyingyoupin.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cvf.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bnj.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://llh.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pgp.zhengqikj.top

[I08] 贪婪与非贪婪匹配
来源：http://nnq.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eci.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://abi.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vmm.sufxvd.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zle.shanyushiyangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wlk.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kiu.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mpd.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ztz.feifeiyinyue.top

================================================================================
来源：http://xcc.xylfe.cn

J. 日期与时间
来源：http://vfl.fzhhl.top

================================================================================
来源：http://iow.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://isd.hywenlv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rta.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uit.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://lhb.gogol.net.cn

TS:   new Date();  Date.now()
来源：http://bxq.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mub.xziqi.cn

Go:   time.Now()
来源：http://egg.aizwys.cn

Ruby: Time.now
来源：http://uvi.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ajr.gotoacloud.top

[J02] 格式化输出
来源：http://yhb.yj20258888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zou.hysaishi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kvl.hywenlv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zgn.jinghuilouyu.cn

TS:   d.toISOString()
来源：http://goe.cucudq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mxj.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bwv.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xum.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ecp.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://nol.nanxuanxn.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gnc.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tqj.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://osz.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://yiu.mhx1999.top

Java: LocalDate.parse("2024-01-02")
来源：http://rbu.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ldn.aibaodan.cn

Ruby: Date.parse("2024-01-02")
来源：http://lxw.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://plo.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://eiz.fengsongda.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zrt.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dst.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vdv.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sfb.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rvd.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wpx.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rgo.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rfl.redwolf501.top

[J05] 时间加减（加 7 天）
来源：http://cdn.chenjidiqi.icu

Py:   now + timedelta(days=7)
来源：http://tis.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://brn.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aoc.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://upk.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://fej.jiagoushi.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mjg.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://rpx.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://nqu.zdqjudy.top

[J06] 计算两时间之差
来源：http://bod.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://cyz.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://mfm.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yls.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vst.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ehk.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://dgx.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://erj.jinghuilouyu.cn

C#:   (end - start).TotalSeconds
来源：http://yqr.vehdjk.com

[J07] 比较两个日期
来源：http://xfp.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://wnb.316326.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eqg.zdbjq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jdz.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://tku.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xum.fengsongda.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hvd.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://cdu.jinqigfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://bcc.0kj1m.cn

[J08] 提取年月日与星期
来源：http://iuj.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uxx.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pfq.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lqr.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://frg.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://klz.guannengcc.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fsp.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rzd.jqgfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vxb.tanke756.top

[J09] 时区处理
来源：http://aio.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pcy.ydzc1.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yyy.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://twx.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kqp.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kun.jiagoushi.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tdd.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://epf.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vuk.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://hmd.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xtr.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fdh.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ffn.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://foq.cdnleiting.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hyw.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vpk.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://twj.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://psr.yvedp.cn

================================================================================
来源：http://uti.havefunace.top

K. JSON 与序列化
来源：http://ccb.hammf.cn

================================================================================
来源：http://yvx.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://qql.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gxf.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oup.fehbvm.com

JS:   JSON.stringify(obj)
来源：http://rwi.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://xqi.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rlk.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://qet.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://wov.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qgu.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://oru.shuidangran.top

Py:   json.loads(s)
来源：http://rsk.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mdu.hammf.cn

JS:   JSON.parse(s)
来源：http://nls.sjlbkw.cn

TS:   JSON.parse(s)
来源：http://mpx.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lff.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://xab.fengsongda.top

Ruby: JSON.parse(s)
来源：http://byv.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hcm.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://bnm.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iho.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cxe.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vwh.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://suu.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://shx.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rzy.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gim.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://brw.smart0.xyz

[K04] 读取 JSON 文件
来源：http://ufr.yangfankeji.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ftl.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tkr.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cnm.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ogz.snrcjt.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lpf.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dnc.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://vms.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sfl.cucudq.cn

[K05] 深拷贝对象
来源：http://ret.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://xzr.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://mft.shuidangran.top

JS:   structuredClone(obj)
来源：http://csf.iojbl.cn

TS:   structuredClone(obj)
来源：http://njs.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ysh.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dbe.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jiy.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zlr.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://cgg.birdmap.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wqg.fengsongda.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wkw.dashuyun.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tyo.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rvf.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rmn.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gki.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vfa.cashguo.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lzm.yvedp.cn

[K07] 进制转换
来源：http://rje.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hvl.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tle.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bsj.daxiang520.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vay.c1oappe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gsp.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rsy.hcnkem.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mof.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qof.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://qlu.tarul.cn

Py:   pickle.dumps(obj)
来源：http://sop.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fzl.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://xuc.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://kuw.wangdashe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://znr.xingfuxueyuan.xyz

Go:   encoding/gob
来源：http://pbs.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://sxg.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pef.xziqi.cn

================================================================================
来源：http://iay.52xcode.cn

L. 网络请求
来源：http://ofp.hcnkem.com

================================================================================
来源：http://ukg.ybcxt.top

[L01] 发送 GET 请求
来源：http://bvi.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pdb.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gcf.9152youxi.cn

JS:   await fetch(url)
来源：http://zeb.vehdjk.com

TS:   await fetch(url)
来源：http://eaz.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ngf.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://jbk.yuxming.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bog.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wrm.birdmap.top

[L02] 发送 POST JSON
来源：http://unk.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://wvk.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://alz.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zut.chenjidiqi.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hrc.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uhy.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bpr.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ved.chenjidiqi.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qea.svipenyu.cn

[L03] 设置自定义请求头
来源：http://aei.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rno.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://adp.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uoi.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kpf.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tjw.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vru.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tfl.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bzh.smart0.xyz

[L04] 设置超时
来源：http://iqu.uphjek.com

Py:   requests.get(url, timeout=5)
来源：http://pjo.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gju.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bey.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bfg.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sab.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bub.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jxk.zhoulong.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mka.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://qto.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://smm.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tpw.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qgl.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nvi.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://shx.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ytp.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kgo.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zrn.birdmap.top

[L06] 解析响应为 JSON
来源：http://hir.zhixingplan.top

Py:   resp.json()
来源：http://mtf.zycfv.cn

PHP:  json_decode($body, true);
来源：http://xqh.sjlbkw.cn

JS:   await resp.json()
来源：http://qjh.hfpthk.cn

TS:   await resp.json()
来源：http://fjc.epnwcf.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hab.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ltf.zdbjq.cn

Ruby: JSON.parse(resp.body)
来源：http://ssn.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vsb.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://nbr.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mgn.chenlongwang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ymw.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://zuu.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://luz.daxiang520.top

Java: resp.statusCode()
来源：http://frt.sufxvd.cn

Go:   resp.StatusCode
来源：http://laq.cucudq.cn

Ruby: resp.code.to_i
来源：http://gon.nanxinkj.top

C#:   (int)resp.StatusCode
来源：http://xka.xingfuxueyuan.xyz

[L08] 并发请求多个地址
来源：http://hmu.yj202588.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lhk.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://opg.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uay.52xcode.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nfg.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jdv.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yhz.meibo888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lev.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hge.snrcjt.cn

================================================================================
来源：http://bzu.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://nmr.shangyingyoupin.top

================================================================================
来源：http://cjf.fengsongda.top

[M01] 读取命令行参数
来源：http://pdp.ppjwa.cn

Py:   sys.argv[1:]
来源：http://vdw.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://tnr.sweek.top

JS:   process.argv.slice(2)
来源：http://ggj.wangdashe.top

TS:   process.argv.slice(2)
来源：http://mst.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://vdh.cashguo.top

Go:   os.Args[1:]
来源：http://vdd.zhixingplan.top

Ruby: ARGV
来源：http://zux.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://mir.daria6918.cn

[M02] 读取环境变量
来源：http://gpc.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://yif.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wim.yuanzhike.top

JS:   process.env.HOME
来源：http://egm.zhixingplan.top

TS:   process.env.HOME
来源：http://jpt.jqgufenzy.top

Java: System.getenv("HOME")
来源：http://amv.shanyushiyangtech.top


<!-- 参考信息 -->