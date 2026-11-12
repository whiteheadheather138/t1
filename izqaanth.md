代发 wailian999

Ruby: super
来源：http://dti.yanxiufei.cn

C#:   base.Greet();
来源：http://cye.zhongyouzk.top

[G08] 静态方法与属性
来源：http://jvs.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hvs.jinqigfzy.top

PHP:  public static function f() {}
来源：http://lzk.cqqwz.cn

JS:   static f() {}
来源：http://inm.zhiwuduotai.top

TS:   static f(): void {}
来源：http://xni.yuanzhike.top

Java: static void f() {}
来源：http://hck.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bmc.wangdashe.top

Ruby: def self.f; end
来源：http://kbv.jinqigufen.top

C#:   public static void F() {}
来源：http://kdt.pycfn.com

[G09] 接口 / 抽象类
来源：http://uri.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://rhq.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://wub.gzhubu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xwx.andypj.xyz

TS:   interface Shape { area(): number; }
来源：http://ykm.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://sgs.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://okn.tarul.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cds.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://wkx.sjlbkw.cn

[G10] 访问控制
来源：http://drh.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://ios.xylfe.cn

PHP:  public / protected / private
来源：http://ocl.iojbl.cn

JS:   #private 字段；其余公开
来源：http://ocy.ydzc1.top

TS:   public / protected / private
来源：http://dyj.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://szp.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://edw.svipenyu.cn

Ruby: public / protected / private
来源：http://xhz.jqgufenzy.top

C#:   public / protected / private / internal
来源：http://hvy.redwolf501.top

[G11] getter / setter
来源：http://tdh.xylfe.cn

Py:   @property 与 @x.setter
来源：http://akv.0kj1m.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uqj.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://qai.ppjwa.cn

TS:   get name(): string { return this._name; }
来源：http://uir.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://tqh.yuxming.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://luw.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://zkj.yj20258888.top

C#:   public string Name { get; set; }
来源：http://gwu.redwolf501.top

[G12] 对象转字符串
来源：http://lbd.fehbvm.com

Py:   def __str__(self): return self.name
来源：http://rko.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mpb.birdmap.top

JS:   toString() { return this.name; }
来源：http://tjd.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://bgp.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://hqe.pycfn.com

Go:   func (u User) String() string { return u.Name }
来源：http://mfd.dashuyun.cn

Ruby: def to_s; @name; end
来源：http://ezv.ivvv.top

C#:   public override string ToString() => Name;
来源：http://aua.yuxming.cn

[G13] 判断对象类型
来源：http://fps.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://htz.cashguo.top

PHP:  $u instanceof User
来源：http://muu.jianghu66.top

JS:   u instanceof User
来源：http://vic.ehwqpu.com

TS:   u instanceof User
来源：http://oii.dianchejie.cn

Java: u instanceof User
来源：http://czm.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ayr.pengpengdd.cyou

Ruby: u.is_a?(User)
来源：http://row.cdnleiting.top

C#:   u is User
来源：http://ans.hnxiangtu.top

[G14] 数据类 / record
来源：http://szo.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ocf.cdnleiting.top

PHP:  // 用 readonly 属性模拟
来源：http://voy.mhx1999.top

JS:   // 无内置：普通类或对象字面量
来源：http://sxe.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://tlj.redwolf501.top

Java: record User(String name, int age) {}
来源：http://vew.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://cnk.cashguo.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sic.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://khb.sweek.top

[G15] 枚举
来源：http://myc.shanyushiyangtech.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pzf.jinghuilouyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://efi.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fea.yongpay.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jhy.hammf.cn

Java: enum Color { RED, GREEN }
来源：http://igf.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hbk.chenjidiqi.icu

Ruby: Color = %i[red green].freeze
来源：http://zfk.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nyi.yonumen.top

[G16] 对象转数组 / 字典
来源：http://dba.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ywn.fktsv.cn

PHP:  get_object_vars($obj);
来源：http://efv.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://kdn.zycfv.cn

TS:   Object.entries(obj)
来源：http://oqs.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ssh.ywan-chungtsiang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://upc.zhengqikj.top

Ruby: obj.instance_variables
来源：http://itt.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://dum.vehdjk.com

================================================================================
来源：http://pjr.yj20258.top

H. 异常与错误处理
来源：http://jgx.zhengqikj.top

================================================================================
来源：http://zxs.xuanzx.com

[H01] try / catch 基础
来源：http://xsk.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xgy.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zru.ywan-chungtsiang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rpe.snrcjt.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://spi.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yjy.cqqwz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wrq.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hgt.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lym.sweek.top

[H02] finally / ensure 收尾
来源：http://skc.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://xdl.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pjg.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fgn.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ifs.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://opp.316326.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://eoh.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://eiy.epnwcf.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://pkd.gotoacloud.top

[H03] 主动抛出异常
来源：http://sxe.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://krx.vqdsnc.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://msg.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://kpt.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://oot.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bmo.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fob.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gww.fehbvm.com

C#:   throw new ArgumentException("错误信息");
来源：http://gsw.tian-w.cn

[H04] 自定义异常类型
来源：http://fkg.yongpay.top

Py:   class MyError(Exception): pass
来源：http://uyu.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://gmh.yueranfly.top

JS:   class MyError extends Error {}
来源：http://erl.xinyue.icu

TS:   class MyError extends Error {}
来源：http://ukr.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://uph.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pyr.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://lyy.bjfxy.top

C#:   class MyException : Exception {}
来源：http://jsj.guowangkeji.top

[H05] 捕获特定类型
来源：http://euv.wangshuangyany.cn

Py:   except ValueError as e:
来源：http://kkw.hywenlv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tis.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://tsx.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://djr.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://ymx.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ebq.jinqigufen.top

Ruby: rescue ArgumentError => e
来源：http://plg.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lia.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://nrl.yvedp.cn

Py:   value = d.get("k") or default
来源：http://sxh.sufxvd.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sio.jianghu66.top

JS:   obj?.a?.b;  d ?? default
来源：http://guk.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://wym.feifeiyinyue.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nyq.daria6918.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://paf.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://kun.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://pxi.jyoumei.cn

[H07] 断言
来源：http://pqh.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://rct.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://jdu.cucudq.cn

JS:   console.assert(x > 0);
来源：http://tla.nwbrower.top

TS:   console.assert(x > 0);
来源：http://puu.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://byc.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zex.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://spl.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://xst.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://mtu.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://mly.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mjv.fktsv.cn

JS:   e.message;  e.stack
来源：http://jgq.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qsy.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://oln.sxryk.cn

Go:   err.Error()
来源：http://pqd.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://bge.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://ybz.iojbl.cn

[H09] 带错误码的异常
来源：http://iax.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pkg.zdqjudy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://agv.jqgufenzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gyl.tianlin.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gry.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xyg.gotoacloud.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gnd.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://wro.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fyq.bjfxy.top

[H10] 资源自动释放
来源：http://zay.xinyue.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://tzj.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gzt.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://liq.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wso.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zew.gotoacloud.top

Go:   defer f.Close()
来源：http://vlv.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://weg.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hja.ivvv.top

================================================================================
来源：http://fll.zhiwuduotai.top

I. 正则表达式
来源：http://qjj.nanxuanxn.top

================================================================================
来源：http://jok.zhijiandao.cn

[I01] 判断是否匹配
来源：http://kkm.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://plp.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://mtr.wangdashe.top

JS:   /\d+/.test(s)
来源：http://per.fehbvm.com

TS:   /\d+/.test(s)
来源：http://grs.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eiu.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://muz.hfpthk.cn

Ruby: s.match?(/\d+/)
来源：http://kve.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://smb.nanxinkj.top

[I02] 提取所有匹配
来源：http://pql.tanke756.top

Py:   re.findall(r"\d+", s)
来源：http://pfa.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ejp.sysykeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yyx.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://sgv.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iyj.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hid.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://exu.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hud.yuanzhike.top

[I03] 提取捕获分组
来源：http://exi.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jcs.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://our.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kxv.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sen.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xar.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kvj.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wpg.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lrm.tanke756.top

[I04] 正则替换
来源：http://ups.meibo888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wow.xuanzx.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qyg.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://cdr.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://urh.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://qto.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lfk.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ocv.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yxm.ybcxt.top

[I05] 按正则拆分
来源：http://blc.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hto.zhaomingkeji.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dac.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://wlz.cheryme.top

TS:   s.split(/\s*,\s*/)
来源：http://ojy.hfpthk.cn

Java: s.split("\\s*,\\s*")
来源：http://rke.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yns.tanke756.top

Ruby: s.split(/\s*,\s*/)
来源：http://yjf.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qvm.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eds.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sys.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kkk.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bou.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hms.zycfv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wsa.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lnb.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://err.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://arc.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://uoq.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dls.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://djv.gaohongyu789.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lfz.guannengcc.top

TS:   /error/gim
来源：http://vie.ydzc1.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dum.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ktu.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://gma.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://osy.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://ejk.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://boq.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qtc.bbcook.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wkv.haohaochexian.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://luf.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xpy.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bug.smart0.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hts.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nhn.guowangkeji.top

================================================================================
来源：http://aqo.meibo888.top

J. 日期与时间
来源：http://gue.zhixingplan.top

================================================================================
来源：http://iae.dashuyun.cn

[J01] 获取当前时间
来源：http://ycw.aibaodan.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vqw.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://win.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://zzt.xuanzx.com

TS:   new Date();  Date.now()
来源：http://lus.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kyt.vqdsnc.cn

Go:   time.Now()
来源：http://aik.xinyue.icu

Ruby: Time.now
来源：http://tgl.tianlin.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jxm.vqdsnc.cn

[J02] 格式化输出
来源：http://smb.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yro.zhixingplan.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yvr.xziqi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mjo.quarkkingdee.top

TS:   d.toISOString()
来源：http://dmr.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zar.shuidangran.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://whp.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jcg.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://udp.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://mzj.cdnleiting.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://djd.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jko.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://htf.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://hga.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zml.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wlr.gotoacloud.top

Ruby: Date.parse("2024-01-02")
来源：http://gvm.jinqigufen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wir.c1oappe.top

[J04] 时间戳与日期互转
来源：http://zil.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://khh.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oqj.smart0.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xdq.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://gre.zhaomingkeji.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bly.bbcook.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kco.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gck.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dyd.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://tvm.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://asd.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tne.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pjp.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://psv.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://hrs.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vyc.jinqigfzy.top

Ruby: Time.now + 7 * 86400
来源：http://xgl.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://xfh.guannengcc.top

[J06] 计算两时间之差
来源：http://iwj.bbcook.cn


<!-- 参考信息 -->