代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://ysn.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://ppn.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://stg.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://grl.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://ota.cashguo.top

[G07] 调用父类方法
来源：http://sjr.hywenlv.cn

Py:   super().greet()
来源：http://msd.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://uxp.cdnleiting.top

JS:   super.greet();
来源：http://wks.pengpengdd.cyou

TS:   super.greet();
来源：http://xkm.sxryk.cn

Java: super.greet();
来源：http://ghz.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://img.jianghu66.top

Ruby: super
来源：http://aye.gotoacloud.top

C#:   base.Greet();
来源：http://qmw.shzxlz.cn

[G08] 静态方法与属性
来源：http://bbc.wangdashe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lcq.gogol.net.cn

PHP:  public static function f() {}
来源：http://sya.shuidangran.top

JS:   static f() {}
来源：http://fua.yueranfly.top

TS:   static f(): void {}
来源：http://hhi.jinqigfzy.top

Java: static void f() {}
来源：http://zkv.zhoulong.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://vac.sysykeji.top

Ruby: def self.f; end
来源：http://aps.shangyingyoupin.top

C#:   public static void F() {}
来源：http://tfo.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://rco.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://cbb.haohaochexian.top

PHP:  interface Shape { public function area(): float; }
来源：http://ocj.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bmk.chenlongwang.top

TS:   interface Shape { area(): number; }
来源：http://ckn.vehdjk.com

Java: interface Shape { double area(); }
来源：http://rbh.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://rqv.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xpa.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://kop.birdmap.top

[G10] 访问控制
来源：http://ngh.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://qlt.meibo888.top

PHP:  public / protected / private
来源：http://kgo.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://ucm.tianlin.xyz

TS:   public / protected / private
来源：http://fvv.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://lak.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://xit.zhiwuduotai.top

Ruby: public / protected / private
来源：http://xiv.zdbjq.cn

C#:   public / protected / private / internal
来源：http://ypk.fktsv.cn

[G11] getter / setter
来源：http://lxu.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://dkw.c1oappe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tso.guowangkeji.top

JS:   get name() { return this._name; }
来源：http://ief.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://wvl.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://qzy.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fcv.aizwys.cn

Ruby: attr_accessor :name
来源：http://dxj.meibo888.top

C#:   public string Name { get; set; }
来源：http://lcd.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://ati.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://twk.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://erm.yfazqb.com

JS:   toString() { return this.name; }
来源：http://syc.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://byl.yj202588.top

Java: @Override public String toString() { return name; }
来源：http://gim.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://jwu.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://dki.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://deu.yueranfly.top

[G13] 判断对象类型
来源：http://roi.xinyue.icu

Py:   isinstance(u, User)
来源：http://mbd.hesvh.cn

PHP:  $u instanceof User
来源：http://azu.feifeiyinyue.top

JS:   u instanceof User
来源：http://jqq.fengsongda.top

TS:   u instanceof User
来源：http://gge.shanyushiyangkeji.top

Java: u instanceof User
来源：http://asp.tian-w.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aqk.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://yqy.havefunace.top

C#:   u is User
来源：http://hfw.daxiang520.top

[G14] 数据类 / record
来源：http://mku.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xef.cdnleiting.top

PHP:  // 用 readonly 属性模拟
来源：http://ytn.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kyx.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://vuj.shanyushiyangtech.top

Java: record User(String name, int age) {}
来源：http://ybj.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://igt.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bot.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://cab.zhixingplan.top

[G15] 枚举
来源：http://azb.mhx1999.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tmg.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gps.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://grz.shuidangran.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qnx.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://jzr.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xbj.jqgufenzy.top

Ruby: Color = %i[red green].freeze
来源：http://pcq.zycfv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bgf.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://zir.yuanzhike.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gsa.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://mha.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://ayg.fengsongda.top

TS:   Object.entries(obj)
来源：http://pti.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mng.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zzz.yj20258888.top

Ruby: obj.instance_variables
来源：http://tcr.sxryk.cn

C#:   // 用反射或 System.Text.Json
来源：http://fyw.yueranfly.top

================================================================================
来源：http://gag.hongshengwenyu.top

H. 异常与错误处理
来源：http://rso.andypj.xyz

================================================================================
来源：http://wpc.sufxvd.cn

[H01] try / catch 基础
来源：http://vqy.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ita.ybcxt.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ebv.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kas.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gtq.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kum.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rke.zdqjudy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://luv.yueranfly.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qjg.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://cew.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://duq.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://jay.jianghu66.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yih.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://prd.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jxm.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pvw.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wri.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ncu.jqgfzy.top

[H03] 主动抛出异常
来源：http://qow.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://vbp.jianghu66.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lpe.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://iud.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://jda.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dvd.jinqigufen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fuk.yangfankeji.com

Ruby: raise ArgumentError, "错误信息"
来源：http://gzw.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://nil.yueranfly.top

[H04] 自定义异常类型
来源：http://usn.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://zav.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ltg.feifeiyinyue.top

JS:   class MyError extends Error {}
来源：http://guv.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://xmg.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://utd.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vps.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://ftg.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://csq.shanyushiyangtech.top

[H05] 捕获特定类型
来源：http://wci.mhx1999.top

Py:   except ValueError as e:
来源：http://oua.xinyue.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yfc.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://ncy.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://xzg.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://fth.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cxx.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://qrb.haohaochexian.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bhs.chenzaomai.com

[H06] 可选值 / 空值安全访问
来源：http://eeq.sweek.top

Py:   value = d.get("k") or default
来源：http://upv.wangdashe.top

PHP:  $v = $d["k"] ?? null;
来源：http://vnr.bjfxy.top

JS:   obj?.a?.b;  d ?? default
来源：http://vem.bbcook.cn

TS:   obj?.a?.b;  d ?? default
来源：http://img.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dfs.sjlbkw.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fzb.uphjek.com

Ruby: d&.dig(:a, :b)
来源：http://cyq.xuetiantiany.cn

C#:   obj?.A?.B ?? default
来源：http://kgg.epnwcf.com

[H07] 断言
来源：http://cqf.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://fld.gaohongyu789.top

PHP:  assert($x > 0);
来源：http://ggp.cucudq.cn

JS:   console.assert(x > 0);
来源：http://rwn.fengsongda.top

TS:   console.assert(x > 0);
来源：http://stf.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://nlg.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ozl.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://olp.xinyue.icu

C#:   Debug.Assert(x > 0);
来源：http://ynv.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://vij.zycfv.cn

Py:   str(e);  traceback.format_exc()
来源：http://brj.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dzy.haohaochexian.top

JS:   e.message;  e.stack
来源：http://zbf.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://egs.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://ask.ehwqpu.com

Go:   err.Error()
来源：http://spc.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://fee.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://tzt.shzxlz.cn

[H09] 带错误码的异常
来源：http://qxa.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kcs.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jby.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hrp.hywenlv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ofp.jinqigfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fux.epnwcf.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://beu.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://mgt.zdbjq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zho.yueranfly.top

[H10] 资源自动释放
来源：http://dsy.zhiwuduotai.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zpk.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tvj.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dgc.tianlin.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lyl.shangyingyoupin.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fwh.gzhubu.top

Go:   defer f.Close()
来源：http://olm.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mvt.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kjh.xuanzx.com

================================================================================
来源：http://ryg.vehdjk.com

I. 正则表达式
来源：http://ibg.yj202588.top

================================================================================
来源：http://bxg.andypj.xyz

[I01] 判断是否匹配
来源：http://ric.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wbr.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://xso.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://kzu.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://pqb.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uxg.pycfn.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://stt.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://tam.cqqwz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xgn.shanyushiyangkeji.top

[I02] 提取所有匹配
来源：http://zix.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://sbc.quarkkingdee.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ovt.hywenlv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zis.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://bek.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jiz.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gtn.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://kod.sjlbkw.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dlu.yonumen.top

[I03] 提取捕获分组
来源：http://ybf.52xcode.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fwt.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ozk.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tlv.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jpp.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ewr.smart0.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tmt.yueranfly.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fyy.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://olu.jyoumei.cn

[I04] 正则替换
来源：http://bbv.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://elf.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rti.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mev.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://tbq.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://whu.ppjwa.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xkp.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rmx.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gqm.pengpengdd.cyou

[I05] 按正则拆分
来源：http://gxt.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bhx.hammf.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kwx.pycfn.com

JS:   s.split(/\s*,\s*/)
来源：http://yis.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://ukr.shanyushiyangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://jdd.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lyw.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://iqq.hcnkem.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://afg.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nem.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ted.zhiwuduotai.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://epm.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eel.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jjq.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fhj.zhengqikj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iwt.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gut.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ckv.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://hgq.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hjs.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aor.hnqzz.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kcd.epnwcf.com

TS:   /error/gim
来源：http://afb.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uxc.birdmap.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://okh.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://qlj.tianlin.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hmj.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://fba.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qlk.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://osc.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vrp.jyoumei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bzt.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://xqz.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vgd.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oia.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jrw.yj202588.top

================================================================================
来源：http://run.shanyushiyangkeji.top

J. 日期与时间
来源：http://zng.hfpthk.cn

================================================================================
来源：http://pzq.jianghu66.top

[J01] 获取当前时间
来源：http://piw.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zut.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jmk.fengsongda.top

JS:   new Date();  Date.now()
来源：http://apo.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://eqx.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pzg.daria6918.cn

Go:   time.Now()
来源：http://ibf.tianlin.xyz

Ruby: Time.now
来源：http://oxc.chenjidiqi.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://evq.jinghuilouyu.cn

[J02] 格式化输出
来源：http://cpj.xingfuxueyuan.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zcu.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://foq.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hog.sufxvd.cn

TS:   d.toISOString()
来源：http://yzq.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kdk.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ode.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xhs.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wgk.hesvh.cn

[J03] 字符串解析为日期
来源：http://dgc.gaohongyu789.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dec.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nqt.xinyue.icu

JS:   new Date("2024-01-02")
来源：http://ugy.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://xra.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://uhd.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bdn.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://bqt.hnqzz.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kky.yonumen.top

[J04] 时间戳与日期互转
来源：http://eek.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nrd.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rvb.chenjidiqi.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cis.jinqigfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vhq.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sew.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uce.dashuyun.cn


<!-- 参考信息 -->