代发 wailian999

PHP:  public static function f() {}
来源：http://ibs.jiagoushi.top

JS:   static f() {}
来源：http://qhi.xuetiantiany.cn

TS:   static f(): void {}
来源：http://ztx.tarul.cn

Java: static void f() {}
来源：http://fou.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bwi.xuanzx.com

Ruby: def self.f; end
来源：http://zll.hnxiangtu.top

C#:   public static void F() {}
来源：http://nrf.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://sms.chenzaomai.com

Py:   from abc import ABC, abstractmethod
来源：http://dnx.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bgt.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kor.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://elj.fktsv.cn

Java: interface Shape { double area(); }
来源：http://hud.yj20258.top

Go:   type Shape interface { Area() float64 }
来源：http://zoe.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bsj.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://tel.52xcode.cn

[G10] 访问控制
来源：http://xxk.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://xxd.yfazqb.com

PHP:  public / protected / private
来源：http://vob.yfazqb.com

JS:   #private 字段；其余公开
来源：http://trv.yangfankeji.com

TS:   public / protected / private
来源：http://ydh.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://yiq.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nus.xuanzx.com

Ruby: public / protected / private
来源：http://auy.xylfe.cn

C#:   public / protected / private / internal
来源：http://akh.hammf.cn

[G11] getter / setter
来源：http://wkq.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://abq.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dwt.bjfxy.top

JS:   get name() { return this._name; }
来源：http://wnp.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://djn.shuidangran.top

Java: public String getName() { return name; }
来源：http://alo.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rlr.pycfn.com

Ruby: attr_accessor :name
来源：http://nzl.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://gvz.c1oappe.top

[G12] 对象转字符串
来源：http://gxr.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://ilx.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lpw.zhongyouzk.top

JS:   toString() { return this.name; }
来源：http://slb.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://sbt.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://zug.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://swu.fzhhl.top

Ruby: def to_s; @name; end
来源：http://uzx.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://bnx.yuxming.cn

[G13] 判断对象类型
来源：http://qmy.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://udv.gotoacloud.top

PHP:  $u instanceof User
来源：http://rnl.hcnkem.com

JS:   u instanceof User
来源：http://rrn.xuanzx.com

TS:   u instanceof User
来源：http://rnb.ppjwa.cn

Java: u instanceof User
来源：http://lop.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ipc.316326.xyz

Ruby: u.is_a?(User)
来源：http://ojr.andypj.xyz

C#:   u is User
来源：http://ljr.haohaochexian.top

[G14] 数据类 / record
来源：http://nzh.yueranfly.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hvy.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://xtj.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://otd.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://xwp.yj20258.top

Java: record User(String name, int age) {}
来源：http://ixm.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://ydw.vehdjk.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dex.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://pip.jiagoushi.top

[G15] 枚举
来源：http://jfl.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lim.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lds.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://duc.aizwys.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jtq.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://yyu.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ihq.jiagoushi.top

Ruby: Color = %i[red green].freeze
来源：http://tiq.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vps.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://pdw.yj20258.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bbz.chenzaomai.com

PHP:  get_object_vars($obj);
来源：http://wvy.andypj.xyz

JS:   Object.entries(obj)
来源：http://zpq.mhx1999.top

TS:   Object.entries(obj)
来源：http://rqs.havefunace.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tie.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ofn.nwbrower.top

Ruby: obj.instance_variables
来源：http://oes.zhaomingkeji.xyz

C#:   // 用反射或 System.Text.Json
来源：http://tmx.fzhhl.top

================================================================================
来源：http://yod.jqgfzy.top

H. 异常与错误处理
来源：http://tgh.svipenyu.cn

================================================================================
来源：http://shj.jianghu66.top

[H01] try / catch 基础
来源：http://okv.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jqm.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gfr.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xhv.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://deo.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://som.sxryk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tgq.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hxm.yueranfly.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fbo.hnqzz.top

[H02] finally / ensure 收尾
来源：http://ogj.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://dnp.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mtc.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pog.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ieq.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bgu.fehbvm.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://poz.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hut.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dkk.zhengqikj.top

[H03] 主动抛出异常
来源：http://brm.shangyingyoupin.top

Py:   raise ValueError("错误信息")
来源：http://vtk.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lje.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://rbj.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://fvp.xuanzx.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://edo.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://afl.aibaodan.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lms.aizwys.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oob.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://xwh.yfazqb.com

Py:   class MyError(Exception): pass
来源：http://rqw.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bdh.snrcjt.cn

JS:   class MyError extends Error {}
来源：http://sbs.hcnkem.com

TS:   class MyError extends Error {}
来源：http://vfx.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://lul.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ruf.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://izq.yj202588.top

C#:   class MyException : Exception {}
来源：http://xfq.nanxuanxn.top

[H05] 捕获特定类型
来源：http://mnj.hcnkem.com

Py:   except ValueError as e:
来源：http://vyc.xuanzx.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yqn.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://oon.jianghu66.top

TS:   if (e instanceof TypeError) {}
来源：http://etv.yvedp.cn

Java: catch (IOException | SQLException e) {}
来源：http://ste.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bub.daxiang520.top

Ruby: rescue ArgumentError => e
来源：http://hiv.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cbo.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://ano.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://bfc.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://dfv.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mqr.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sks.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hmo.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://evo.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://yhj.0kj1m.cn

C#:   obj?.A?.B ?? default
来源：http://keu.zdqjudy.top

[H07] 断言
来源：http://wek.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://pce.hammf.cn

PHP:  assert($x > 0);
来源：http://chs.jqgufenzy.top

JS:   console.assert(x > 0);
来源：http://rhn.jinqigufen.top

TS:   console.assert(x > 0);
来源：http://ewe.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://tfx.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ewp.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://qjw.daria6918.cn

C#:   Debug.Assert(x > 0);
来源：http://ldz.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://tln.yvedp.cn

Py:   str(e);  traceback.format_exc()
来源：http://jex.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dfl.sjlbkw.cn

JS:   e.message;  e.stack
来源：http://vxw.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://srm.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pgi.snrcjt.cn

Go:   err.Error()
来源：http://qjo.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://wfp.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://vnb.bbcook.cn

[H09] 带错误码的异常
来源：http://scr.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bds.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://imq.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://agf.fanxiaobao.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://coj.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nsd.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://itt.fanxiaobao.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ype.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fuf.redwolf501.top

[H10] 资源自动释放
来源：http://iws.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://jrn.ydzc1.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://luv.aibaodan.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fsi.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bvg.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cub.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://tcj.chenjidiqi.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bsv.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://umr.shuidangran.top

================================================================================
来源：http://teo.fzhhl.top

I. 正则表达式
来源：http://mzt.yueranfly.top

================================================================================
来源：http://iey.shangyingyoupin.top

[I01] 判断是否匹配
来源：http://inp.jlsjyb.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dzi.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ikr.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://yus.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://tit.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ppt.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lbi.316326.xyz

Ruby: s.match?(/\d+/)
来源：http://ywc.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fcx.chenjidiqi.icu

[I02] 提取所有匹配
来源：http://unz.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://ndf.yangfankeji.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tmp.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mjg.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://fin.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://khx.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://osv.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://sso.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ofo.hywenlv.cn

[I03] 提取捕获分组
来源：http://otx.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xpp.bjfxy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://buf.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qqk.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rms.aibaodan.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sor.yfazqb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aaj.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tdm.cucudq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jhl.ybcxt.top

[I04] 正则替换
来源：http://twn.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://szj.daxiang520.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wnz.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zjr.havefunace.top

TS:   s.replace(/\d+/g, "#")
来源：http://wed.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://czb.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gda.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jqz.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://okb.9152youxi.cn

[I05] 按正则拆分
来源：http://gfd.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bma.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zpt.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://yny.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://hps.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://nyo.tanke756.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yyz.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://ajt.chenzaomai.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zyl.zhijiandao.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ief.sxryk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cpa.hammf.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pzi.quarkkingdee.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nip.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://enz.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xkt.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pya.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://efc.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rnc.aibaodan.cn

[I07] 忽略大小写与多行模式
来源：http://mgn.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lpl.yonumen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pwn.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aqz.hongshengwenyu.top

TS:   /error/gim
来源：http://lxl.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tnb.xziqi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jeu.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://uub.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vpa.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://omd.hnqzz.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rtl.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ziy.ehwqpu.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mvw.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sdg.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gny.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hkw.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qow.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ujs.yvedp.cn

================================================================================
来源：http://zuu.tanke756.top

J. 日期与时间
来源：http://foz.yangfankeji.com

================================================================================
来源：http://zoi.yj202588.top

[J01] 获取当前时间
来源：http://rps.kuanghao11.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ymc.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hrh.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://mcc.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://mhd.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://grp.zhongyouzk.top

Go:   time.Now()
来源：http://iiy.wangshuangyany.cn

Ruby: Time.now
来源：http://fqq.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kzy.0kj1m.cn

[J02] 格式化输出
来源：http://erl.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jhi.cashguo.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://idu.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://drt.shuidangran.top

TS:   d.toISOString()
来源：http://dca.snrcjt.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cae.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rpw.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cfw.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qoy.nanxinkj.top

[J03] 字符串解析为日期
来源：http://nfo.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tcl.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tcr.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://usv.birdmap.top

TS:   new Date("2024-01-02")
来源：http://iws.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ydn.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lcg.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://xqv.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lug.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://wuo.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wes.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ozg.yj202588.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kia.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://izr.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ytz.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yht.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yyp.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gxj.yongpay.top

[J05] 时间加减（加 7 天）
来源：http://bcl.xuanzx.com

Py:   now + timedelta(days=7)
来源：http://qvb.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://xmn.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jbp.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mqp.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://fzq.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ecm.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://qfe.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://knb.sweek.top

[J06] 计算两时间之差
来源：http://puq.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://wcd.gaohongyu789.top

PHP:  $end->diff($start)->days;
来源：http://lgh.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vmy.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hsu.zhijiandao.cn


<!-- 参考信息 -->