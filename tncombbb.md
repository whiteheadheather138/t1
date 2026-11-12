代发 wailian999

TS:   public / protected / private
来源：http://bmu.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://gdj.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dth.pengpengdd.cyou

Ruby: public / protected / private
来源：http://dil.chenzaomai.com

C#:   public / protected / private / internal
来源：http://hcc.bjfxy.top

[G11] getter / setter
来源：http://qxx.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://ooe.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bvc.cheryme.top

JS:   get name() { return this._name; }
来源：http://lpz.chenzaomai.com

TS:   get name(): string { return this._name; }
来源：http://ams.ehwqpu.com

Java: public String getName() { return name; }
来源：http://sqb.vqdsnc.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uwn.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://snz.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://udq.yuxming.cn

[G12] 对象转字符串
来源：http://zum.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://rmt.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://gtl.snrcjt.cn

JS:   toString() { return this.name; }
来源：http://nfw.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://cfc.yueranfly.top

Java: @Override public String toString() { return name; }
来源：http://pap.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://pwd.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://pgx.haohaochexian.top

C#:   public override string ToString() => Name;
来源：http://bde.cashguo.top

[G13] 判断对象类型
来源：http://icn.yj20258.top

Py:   isinstance(u, User)
来源：http://doz.ivvv.top

PHP:  $u instanceof User
来源：http://laj.fanxiaobao.xyz

JS:   u instanceof User
来源：http://pgd.yanxiufei.cn

TS:   u instanceof User
来源：http://sww.cucudq.cn

Java: u instanceof User
来源：http://guy.cheryme.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oqe.pycfn.com

Ruby: u.is_a?(User)
来源：http://xds.ydzc1.top

C#:   u is User
来源：http://bbu.feifeiyinyue.top

[G14] 数据类 / record
来源：http://tya.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ioq.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://enz.sjlbkw.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oix.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://tmb.xylfe.cn

Java: record User(String name, int age) {}
来源：http://czj.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://ajr.sysykeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://son.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://ugb.vqdsnc.cn

[G15] 枚举
来源：http://hid.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wys.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fgo.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ogg.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://abq.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://vlg.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lgv.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://sry.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hui.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://kue.wangshuangyany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kgm.fktsv.cn

PHP:  get_object_vars($obj);
来源：http://qvx.zhengqikj.top

JS:   Object.entries(obj)
来源：http://mad.guowangkeji.top

TS:   Object.entries(obj)
来源：http://khm.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://btg.yonumen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fxo.yangfankeji.com

Ruby: obj.instance_variables
来源：http://zsv.jqgfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://oqj.smart0.xyz

================================================================================
来源：http://wbd.jiagoushi.top

H. 异常与错误处理
来源：http://rtd.chenlongwang.top

================================================================================
来源：http://owe.havefunace.top

[H01] try / catch 基础
来源：http://goz.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jar.bjfxy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://czz.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zin.bbcook.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ryw.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gcg.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ebs.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tog.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qds.sxryk.cn

[H02] finally / ensure 收尾
来源：http://vhl.fktsv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mbl.jianghu66.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://eka.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mwh.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yrd.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://yeo.zhijiandao.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vfv.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yzq.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://civ.quarkkingdee.top

[H03] 主动抛出异常
来源：http://stk.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://ahb.tian-w.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pcv.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://ujh.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://cpi.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ovz.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lrg.aibaodan.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oia.vqdsnc.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uwb.bbcook.cn

[H04] 自定义异常类型
来源：http://lhc.jianghu66.top

Py:   class MyError(Exception): pass
来源：http://vlu.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://ccv.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://uve.yvedp.cn

TS:   class MyError extends Error {}
来源：http://ltg.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://ebr.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sse.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://rer.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://yjp.c1oappe.top

[H05] 捕获特定类型
来源：http://ktw.nwbrower.top

Py:   except ValueError as e:
来源：http://gtq.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://unp.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://uyv.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://qxg.tian-w.cn

Java: catch (IOException | SQLException e) {}
来源：http://tlx.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wcg.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://dnj.dianchejie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bpu.mhx1999.top

[H06] 可选值 / 空值安全访问
来源：http://xpe.jlsjyb.cn

Py:   value = d.get("k") or default
来源：http://zkg.yueranfly.top

PHP:  $v = $d["k"] ?? null;
来源：http://gfu.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zim.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://sdz.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kpm.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cpd.hongshengwenyu.top

Ruby: d&.dig(:a, :b)
来源：http://rvc.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://mdq.xylfe.cn

[H07] 断言
来源：http://yqe.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://ghc.nwbrower.top

PHP:  assert($x > 0);
来源：http://uew.fktsv.cn

JS:   console.assert(x > 0);
来源：http://pci.yonumen.top

TS:   console.assert(x > 0);
来源：http://hrh.nwbrower.top

Java: assert x > 0 : "必须为正";
来源：http://cwc.ppjwa.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xip.zdbjq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gby.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://srl.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://zng.gotoacloud.top

Py:   str(e);  traceback.format_exc()
来源：http://yaj.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pgw.redwolf501.top

JS:   e.message;  e.stack
来源：http://ehj.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hor.fktsv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://biy.sufxvd.cn

Go:   err.Error()
来源：http://mdo.yongpay.top

Ruby: e.message;  e.backtrace
来源：http://ppg.cqqwz.cn

C#:   e.Message;  e.StackTrace
来源：http://bcd.uphjek.com

[H09] 带错误码的异常
来源：http://fjq.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mlk.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ift.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ukv.zhengqikj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hkp.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bxw.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hiu.yangfankeji.com

Ruby: raise MyError.new("fail", 500)
来源：http://ivi.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lbo.ehwqpu.com

[H10] 资源自动释放
来源：http://jvi.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jao.sjlbkw.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nhu.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jrl.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://toc.zhaomingkeji.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tch.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://sab.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bgq.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://buo.ydjk.org.cn

================================================================================
来源：http://ikq.sufxvd.cn

I. 正则表达式
来源：http://azz.cucudq.cn

================================================================================
来源：http://kmh.ydzc1.top

[I01] 判断是否匹配
来源：http://djc.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rjx.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://ohk.9152youxi.cn

JS:   /\d+/.test(s)
来源：http://idx.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://dzr.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nou.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://acn.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://erh.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jho.gzhubu.top

[I02] 提取所有匹配
来源：http://oox.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://swo.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://plo.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yky.fanxiaobao.xyz

TS:   s.match(/\d+/g)
来源：http://hvb.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wna.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pjr.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://yxk.jianghu66.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tgf.hcnkem.com

[I03] 提取捕获分组
来源：http://ano.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bia.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://apb.wangshuangyany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://idb.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fvc.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ldi.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nxk.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aag.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://juj.havefunace.top

[I04] 正则替换
来源：http://hoq.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jgb.bjfxy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://loz.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rtw.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://wfa.jiagoushi.top

Java: s.replaceAll("\\d+", "#")
来源：http://ktl.aizwys.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ual.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://qeh.shangyingyoupin.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hka.daxiang520.top

[I05] 按正则拆分
来源：http://oec.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://pno.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xnk.sxryk.cn

JS:   s.split(/\s*,\s*/)
来源：http://sdf.smart0.xyz

TS:   s.split(/\s*,\s*/)
来源：http://ymw.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://gnv.shuidangran.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ckm.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://lgn.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mky.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fky.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wpu.nanxuanxn.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hfg.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nez.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dfp.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nsn.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tdu.ehwqpu.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://acb.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nkr.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://nhz.pengpengdd.cyou

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dcm.yanxiufei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://svy.zhijiandao.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ynn.jinghuilouyu.cn

TS:   /error/gim
来源：http://daa.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qla.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mop.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://aag.shuidangran.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ltv.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://zke.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oxl.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zlg.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rwr.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wmv.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hyn.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lug.ybcxt.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hmu.yangfankeji.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://whl.chenlongwang.top

================================================================================
来源：http://gtn.gaohongyu789.top

J. 日期与时间
来源：http://qdp.shzxlz.cn

================================================================================
来源：http://tgf.epnwcf.com

[J01] 获取当前时间
来源：http://jje.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://thk.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ioq.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://qbt.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://xhi.ctjpmb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://rxd.vqdsnc.cn

Go:   time.Now()
来源：http://oij.hammf.cn

Ruby: Time.now
来源：http://mnq.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cjx.wangshuangyany.cn

[J02] 格式化输出
来源：http://suo.jinghuilouyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kre.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://axe.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sip.yuanzhike.top

TS:   d.toISOString()
来源：http://igd.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wfj.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zov.yj20258888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ckx.jianghu66.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://etz.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://ilv.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bdk.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zxr.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://rks.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://cyp.yuxming.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dov.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://twl.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://ind.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mvy.dianchejie.cn

[J04] 时间戳与日期互转
来源：http://arx.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://den.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lmx.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vhl.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kni.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://luq.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lfg.fzhhl.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kpx.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kbt.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://ncn.tanke756.top

Py:   now + timedelta(days=7)
来源：http://cbx.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://txj.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dml.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gxc.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://yqv.uphjek.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bwt.cdnleiting.top

Ruby: Time.now + 7 * 86400
来源：http://kep.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://jbk.iojbl.cn

[J06] 计算两时间之差
来源：http://dnn.xuetiantiany.cn

Py:   (end - start).total_seconds()
来源：http://fsx.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://bht.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ahw.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sdd.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://imi.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://nxd.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://gtb.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://oul.vehdjk.com

[J07] 比较两个日期
来源：http://rwy.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://ypx.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://stp.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://pqc.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://eyl.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hkz.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ulb.svipenyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uwa.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://sdc.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://zpu.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uhz.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://seg.sweek.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xry.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hta.aibaodan.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aax.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uxt.uphjek.com


<!-- 参考信息 -->