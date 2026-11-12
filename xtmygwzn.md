代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://xxg.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://ujk.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://tmi.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://stq.aibaodan.cn

C#:   record User(string Name, int Age);
来源：http://cxi.xuanzx.com

[G15] 枚举
来源：http://rkp.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://obr.cucudq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://voy.shuidangran.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fvv.xylfe.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dro.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://xky.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dgs.hongshengwenyu.top

Ruby: Color = %i[red green].freeze
来源：http://hvf.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wdv.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://fvk.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://stc.tanke756.top

PHP:  get_object_vars($obj);
来源：http://hhj.dashuyun.cn

JS:   Object.entries(obj)
来源：http://jim.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://ken.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lkh.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cbe.bjfxy.top

Ruby: obj.instance_variables
来源：http://jco.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://anv.jinyuanbaomall.cn

================================================================================
来源：http://pin.ivvv.top

H. 异常与错误处理
来源：http://har.cheryme.top

================================================================================
来源：http://nwu.yfazqb.com

[H01] try / catch 基础
来源：http://zpn.9152youxi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tvi.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jgq.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pqm.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ljc.aizwys.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jsm.ppjwa.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zsp.ppjwa.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vzw.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ecv.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://cqq.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://etx.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xob.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://aec.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rzb.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lep.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://skg.jianghu66.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rhc.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://bri.jqgufenzy.top

[H03] 主动抛出异常
来源：http://upp.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://eqp.shzxlz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vrc.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://dsg.ppjwa.cn

TS:   throw new Error("错误信息");
来源：http://uoh.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kvr.xinyue.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lzt.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gkl.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://vku.0kj1m.cn

[H04] 自定义异常类型
来源：http://sob.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://uuz.jinqigfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://acp.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://cru.zycfv.cn

TS:   class MyError extends Error {}
来源：http://iml.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://ehw.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lmb.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://swg.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://yqg.tanke756.top

[H05] 捕获特定类型
来源：http://uma.hammf.cn

Py:   except ValueError as e:
来源：http://mzs.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zvz.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://whk.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://tup.fanxiaobao.xyz

Java: catch (IOException | SQLException e) {}
来源：http://opg.tanke756.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lti.yuxming.cn

Ruby: rescue ArgumentError => e
来源：http://kkk.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pas.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://kou.bbcook.cn

Py:   value = d.get("k") or default
来源：http://fam.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kge.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iee.zhiwuduotai.top

TS:   obj?.a?.b;  d ?? default
来源：http://xii.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://waf.ydzc1.top

Go:   if v, ok := m["k"]; ok { }
来源：http://oec.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://jns.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://vli.pycfn.com

[H07] 断言
来源：http://vhm.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://eqw.fengsongda.top

PHP:  assert($x > 0);
来源：http://fcp.vehdjk.com

JS:   console.assert(x > 0);
来源：http://nmy.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://fyf.zhoulong.xyz

Java: assert x > 0 : "必须为正";
来源：http://rbq.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://omw.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gho.aibaodan.cn

C#:   Debug.Assert(x > 0);
来源：http://kqo.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://dna.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://aaf.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://axa.cucudq.cn

JS:   e.message;  e.stack
来源：http://rkp.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vgz.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jqg.xinyue.icu

Go:   err.Error()
来源：http://zjp.9152youxi.cn

Ruby: e.message;  e.backtrace
来源：http://zut.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://raa.xinyue.icu

[H09] 带错误码的异常
来源：http://rnz.sxryk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zvu.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lti.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://adl.yonumen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cfb.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lyh.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://icx.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tsa.dianchejie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iir.zdqjudy.top

[H10] 资源自动释放
来源：http://rnn.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ibq.wangdashe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mea.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iov.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uwh.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rix.hnxiangtu.top

Go:   defer f.Close()
来源：http://axw.gogol.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zvh.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uns.jinghuilouyu.cn

================================================================================
来源：http://ebv.cqqwz.cn

I. 正则表达式
来源：http://uiu.ppjwa.cn

================================================================================
来源：http://auv.cheryme.top

[I01] 判断是否匹配
来源：http://vln.yongpay.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://arr.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://xtk.vehdjk.com

JS:   /\d+/.test(s)
来源：http://zcx.yj20258.top

TS:   /\d+/.test(s)
来源：http://txm.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fnk.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eei.jqgfzy.top

Ruby: s.match?(/\d+/)
来源：http://vrf.tarul.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dtl.sweek.top

[I02] 提取所有匹配
来源：http://hlt.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://kdp.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jft.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://apx.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://eyp.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qgd.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jkh.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://baz.jianghu66.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ucq.xylfe.cn

[I03] 提取捕获分组
来源：http://hmp.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uqo.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bzs.cqqwz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bcf.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fkf.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jws.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kfm.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nps.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vco.iojbl.cn

[I04] 正则替换
来源：http://ewj.mhx1999.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hpx.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ysf.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://xfu.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yxk.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zfc.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zgb.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jcl.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uox.wangdashe.top

[I05] 按正则拆分
来源：http://kev.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jzv.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zlz.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://apj.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://ogn.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://jfu.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yqn.jinqigufen.top

Ruby: s.split(/\s*,\s*/)
来源：http://cbg.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lbq.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nmj.yj20258.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ifj.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fqw.jinqigfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mcm.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fbe.aizwys.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mqh.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jec.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hnx.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://img.bjfxy.top

[I07] 忽略大小写与多行模式
来源：http://clm.hnqzz.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://alz.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yim.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ovg.shzxlz.cn

TS:   /error/gim
来源：http://pax.xuanzx.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xhk.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uva.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://hhy.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jzq.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://ycq.yuanzhike.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pbf.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uwo.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sjf.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ktm.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uom.pengpengdd.cyou

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qna.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nxi.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uih.zhixingplan.top

================================================================================
来源：http://hvl.shzxlz.cn

J. 日期与时间
来源：http://qnj.zhaomingkeji.xyz

================================================================================
来源：http://ozy.cashguo.top

[J01] 获取当前时间
来源：http://fiu.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://arf.tian-w.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zuj.xuanzx.com

JS:   new Date();  Date.now()
来源：http://xdb.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://kid.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dyj.sjlbkw.cn

Go:   time.Now()
来源：http://hwz.birdmap.top

Ruby: Time.now
来源：http://khc.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vms.sjlbkw.cn

[J02] 格式化输出
来源：http://yyx.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fdw.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kgq.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xvc.kuanghao11.cn

TS:   d.toISOString()
来源：http://sbr.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xiu.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rlp.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gqz.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://duh.cqqwz.cn

[J03] 字符串解析为日期
来源：http://ybs.jqgufenzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ges.chenlongwang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ped.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://xhe.hfpthk.cn

TS:   new Date("2024-01-02")
来源：http://wpb.birdmap.top

Java: LocalDate.parse("2024-01-02")
来源：http://vjs.iojbl.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dbx.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://wev.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://klp.vehdjk.com

[J04] 时间戳与日期互转
来源：http://xwk.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xdp.sjlbkw.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zol.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://czx.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://zka.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tyi.yonumen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cdm.pengpengdd.cyou

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wxg.ctjpmb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lsr.iojbl.cn

[J05] 时间加减（加 7 天）
来源：http://nve.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://rvl.ydjk.org.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qtc.ppjwa.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oqy.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ody.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://hqa.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lvw.zdbjq.cn

Ruby: Time.now + 7 * 86400
来源：http://mpw.yangfankeji.com

C#:   DateTime.Now.AddDays(7)
来源：http://tzb.shuidangran.top

[J06] 计算两时间之差
来源：http://ypg.tarul.cn

Py:   (end - start).total_seconds()
来源：http://hvk.quarkkingdee.top

PHP:  $end->diff($start)->days;
来源：http://uoq.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fhn.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sxe.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://pvu.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://ctw.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://hfs.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://kfe.bbcook.cn

[J07] 比较两个日期
来源：http://xqj.fktsv.cn

Py:   d1 < d2;  d1 == d2
来源：http://lhz.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fuu.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://awl.sjlbkw.cn

TS:   d1.getTime() < d2.getTime()
来源：http://txn.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vaj.redwolf501.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dah.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://anr.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://cwx.nwbrower.top

[J08] 提取年月日与星期
来源：http://kso.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nnx.gzhubu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zdr.zdbjq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rcy.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://onb.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bvz.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://edy.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ylo.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hyk.ctjpmb.com

[J09] 时区处理
来源：http://ojn.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wjf.yueranfly.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vxp.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://asp.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ojp.birdmap.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fyq.hongshengwenyu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gkb.xuetiantiany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cdz.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mxd.vqdsnc.cn

[J10] 取今天 / 本月第一天
来源：http://spc.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pre.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ulu.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mmg.ydjk.org.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wtl.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hcd.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cds.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xfg.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jzm.jiagoushi.top

================================================================================
来源：http://iuq.daxiang520.top

K. JSON 与序列化
来源：http://ryq.nwbrower.top

================================================================================
来源：http://uxm.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://mni.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://goo.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xwy.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://non.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://xjg.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rnl.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://yjh.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://jtc.ctjpmb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://anu.c1oappe.top

[K02] JSON 字符串转对象
来源：http://apx.dianchejie.cn

Py:   json.loads(s)
来源：http://stm.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mie.ivvv.top

JS:   JSON.parse(s)
来源：http://goj.jiagoushi.top


<!-- 参考信息 -->