代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://cmr.yonumen.top

JS:   toString() { return this.name; }
来源：http://dbu.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://rgu.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://fsp.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://dcl.dashuyun.cn

Ruby: def to_s; @name; end
来源：http://fwf.yonumen.top

C#:   public override string ToString() => Name;
来源：http://iqb.jlsjyb.cn

[G13] 判断对象类型
来源：http://vni.52xcode.cn

Py:   isinstance(u, User)
来源：http://szl.hammf.cn

PHP:  $u instanceof User
来源：http://abt.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://skg.tian-w.cn

TS:   u instanceof User
来源：http://mrb.zdbjq.cn

Java: u instanceof User
来源：http://lfq.jinqigfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://odx.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://nar.pengpengdd.cyou

C#:   u is User
来源：http://shh.xziqi.cn

[G14] 数据类 / record
来源：http://sag.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nax.gogol.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://rbe.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://ynr.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://xhq.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://ceq.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://hib.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hie.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://gqx.shuidangran.top

[G15] 枚举
来源：http://ndp.bbcook.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zxc.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gwh.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bpb.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yde.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://qds.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gst.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://txl.chenzaomai.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uen.jiagoushi.top

[G16] 对象转数组 / 字典
来源：http://yif.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ffa.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://gwn.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://iko.redwolf501.top

TS:   Object.entries(obj)
来源：http://dtr.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vlz.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sfk.vehdjk.com

Ruby: obj.instance_variables
来源：http://gov.gaohongyu789.top

C#:   // 用反射或 System.Text.Json
来源：http://ynt.zhixingplan.top

================================================================================
来源：http://juc.haohaochexian.top

H. 异常与错误处理
来源：http://ylm.xziqi.cn

================================================================================
来源：http://fmj.chenzaomai.com

[H01] try / catch 基础
来源：http://eje.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hfq.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pbs.yj202588.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bzw.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ryp.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://orx.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zuh.fanxiaobao.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zcn.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lyf.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://ksc.zhixingplan.top

Py:   try: f()⏎finally: cleanup()
来源：http://oio.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gyr.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://faz.birdmap.top

TS:   try { f(); } finally { cleanup(); }
来源：http://txk.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://xlz.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yjn.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fip.nanxinkj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fti.quarkkingdee.top

[H03] 主动抛出异常
来源：http://lll.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://gsv.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zoq.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://exf.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://esc.sweek.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jdn.xylfe.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sae.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ttw.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://xah.fehbvm.com

[H04] 自定义异常类型
来源：http://cnj.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://tsw.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://meg.gzhubu.top

JS:   class MyError extends Error {}
来源：http://rbs.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://irj.hywenlv.cn

Java: class MyException extends RuntimeException {}
来源：http://xjz.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ajs.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://ckz.bbcook.cn

C#:   class MyException : Exception {}
来源：http://nnq.nwbrower.top

[H05] 捕获特定类型
来源：http://nvy.ivvv.top

Py:   except ValueError as e:
来源：http://kbb.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://prb.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://nkm.52xcode.cn

TS:   if (e instanceof TypeError) {}
来源：http://lpg.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://oal.feifeiyinyue.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dqs.havefunace.top

Ruby: rescue ArgumentError => e
来源：http://uta.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ten.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://nyf.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://eid.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://iyw.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://ate.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://euv.yuanzhike.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nvl.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xui.xinyue.icu

Ruby: d&.dig(:a, :b)
来源：http://wuz.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://gwk.zhengqikj.top

[H07] 断言
来源：http://rav.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://fgx.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://wdb.xylfe.cn

JS:   console.assert(x > 0);
来源：http://drm.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://blw.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://yzs.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hgz.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://ack.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://bnw.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://xod.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://xfh.yvedp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://reo.meibo888.top

JS:   e.message;  e.stack
来源：http://pov.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://cfg.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://rlc.jinqigufen.top

Go:   err.Error()
来源：http://frp.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://tfu.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://xnl.kuanghao11.cn

[H09] 带错误码的异常
来源：http://job.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ghn.cheryme.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://trd.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ajf.ydzc1.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mng.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xqx.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ysf.jqgufenzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://tge.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vhy.jlsjyb.cn

[H10] 资源自动释放
来源：http://ddg.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://hnq.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cks.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lve.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cvt.ywan-chungtsiang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cfa.0kj1m.cn

Go:   defer f.Close()
来源：http://mvj.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ydb.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kxo.xuanzx.com

================================================================================
来源：http://ujb.mhx1999.top

I. 正则表达式
来源：http://fjp.shzxlz.cn

================================================================================
来源：http://hoq.tian-w.cn

[I01] 判断是否匹配
来源：http://ggk.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tjw.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qxj.fzhhl.top

JS:   /\d+/.test(s)
来源：http://vlw.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://fby.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jzn.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ftl.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://axt.zycfv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pns.pycfn.com

[I02] 提取所有匹配
来源：http://qnr.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://qds.yj202588.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oke.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lru.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://gie.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rbp.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dnb.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://ttu.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bve.cucudq.cn

[I03] 提取捕获分组
来源：http://cdy.gogol.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vvf.xziqi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jtn.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://svi.ydjk.org.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kcc.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xtx.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iwk.shzxlz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://swv.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://swu.yvedp.cn

[I04] 正则替换
来源：http://ipi.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ogb.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rge.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jhu.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://ril.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://ujq.bbcook.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wvm.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ffb.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vfs.ehwqpu.com

[I05] 按正则拆分
来源：http://ibm.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pww.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pxk.guowangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://igh.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://bgw.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://svl.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uav.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://rom.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wvh.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bxh.tianlin.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yye.hnxiangtu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ptl.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wjv.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://goh.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gkg.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zod.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://btt.hammf.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://irb.uphjek.com

[I07] 忽略大小写与多行模式
来源：http://mgk.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gly.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eqs.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dhz.guannengcc.top

TS:   /error/gim
来源：http://bds.vehdjk.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hxg.epnwcf.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bvk.uphjek.com

Ruby: s.scan(/error/i)
来源：http://rwq.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xht.nanxinkj.top

[I08] 贪婪与非贪婪匹配
来源：http://sci.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rby.gzhubu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jcf.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kmv.ydzc1.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qmv.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ate.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vcm.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aqm.yanxiufei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rhp.andypj.xyz

================================================================================
来源：http://jyq.cucudq.cn

J. 日期与时间
来源：http://vvq.guannengcc.top

================================================================================
来源：http://tom.cdnleiting.top

[J01] 获取当前时间
来源：http://drv.ehwqpu.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://phc.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wkb.zhengqikj.top

JS:   new Date();  Date.now()
来源：http://dum.hcnkem.com

TS:   new Date();  Date.now()
来源：http://erd.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ajo.ctjpmb.com

Go:   time.Now()
来源：http://zwv.sxryk.cn

Ruby: Time.now
来源：http://cka.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qhn.aibaodan.cn

[J02] 格式化输出
来源：http://gfo.chenlongwang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jbv.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ilr.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://agm.sweek.top

TS:   d.toISOString()
来源：http://pjf.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wym.chenzaomai.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ljb.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eta.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wbv.aizwys.cn

[J03] 字符串解析为日期
来源：http://tjd.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gsg.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uox.xinyue.icu

JS:   new Date("2024-01-02")
来源：http://zir.pycfn.com

TS:   new Date("2024-01-02")
来源：http://hvb.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qzo.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rcx.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://qji.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ocd.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://mbl.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xqa.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bbu.tarul.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sjf.yvedp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yjy.jinyuanbaomall.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cph.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tgz.tarul.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yzd.jianghu66.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jvf.yuxming.cn

[J05] 时间加减（加 7 天）
来源：http://zgw.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://igb.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xhw.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pnd.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bsb.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://sbv.shanyushiyangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xah.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://rwn.hongshengwenyu.top

C#:   DateTime.Now.AddDays(7)
来源：http://ped.vqdsnc.cn

[J06] 计算两时间之差
来源：http://xpv.cashguo.top

Py:   (end - start).total_seconds()
来源：http://bww.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://iqo.9152youxi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bvj.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pfi.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://fca.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://zzq.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://nzt.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://xfj.xingfuxueyuan.xyz

[J07] 比较两个日期
来源：http://brb.ctjpmb.com

Py:   d1 < d2;  d1 == d2
来源：http://xel.xinyue.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rhf.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://vhe.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://pex.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ifp.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hph.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://wtk.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://eco.hfpthk.cn

[J08] 提取年月日与星期
来源：http://fyg.feifeiyinyue.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://emu.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hqk.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iww.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oza.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://csj.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jex.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cbo.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vjr.shzxlz.cn

[J09] 时区处理
来源：http://izi.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zgx.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://plz.gogol.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lir.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xhg.wangdashe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fkw.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tfw.ehwqpu.com

Ruby: Time.now.getlocal("+08:00")
来源：http://oso.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qbh.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://hpr.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://blt.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fdi.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xpz.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://edf.bbcook.cn


<!-- 参考信息 -->