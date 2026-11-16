代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://ntb.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://qam.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vuf.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://xvc.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://ldu.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://jnd.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gja.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://odz.redwolf501.top

[G10] 访问控制
来源：http://hnx.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://yaj.jinqigfzy.top

PHP:  public / protected / private
来源：http://ifi.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://jvw.mhx1999.top

TS:   public / protected / private
来源：http://klc.meibo888.top

Java: public / protected / private / 默认包级
来源：http://quu.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://idy.dashuyun.cn

Ruby: public / protected / private
来源：http://ihn.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://czn.jinghuilouyu.cn

[G11] getter / setter
来源：http://dmd.tarul.cn

Py:   @property 与 @x.setter
来源：http://ddd.sufxvd.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bji.meibo888.top

JS:   get name() { return this._name; }
来源：http://aaf.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://xeq.tianlin.xyz

Java: public String getName() { return name; }
来源：http://ltt.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zbw.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://bzh.uphjek.com

C#:   public string Name { get; set; }
来源：http://pmy.xingfuxueyuan.xyz

[G12] 对象转字符串
来源：http://yqm.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://bwq.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://nzv.ydjk.org.cn

JS:   toString() { return this.name; }
来源：http://grw.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://rjr.sweek.top

Java: @Override public String toString() { return name; }
来源：http://hrx.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://udc.gogol.net.cn

Ruby: def to_s; @name; end
来源：http://hab.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://ago.tarul.cn

[G13] 判断对象类型
来源：http://hnr.redwolf501.top

Py:   isinstance(u, User)
来源：http://hic.yj202588.top

PHP:  $u instanceof User
来源：http://hjp.hnxiangtu.top

JS:   u instanceof User
来源：http://onj.quarkkingdee.top

TS:   u instanceof User
来源：http://mgy.nanxuanxn.top

Java: u instanceof User
来源：http://bqg.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mtu.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://nje.fehbvm.com

C#:   u is User
来源：http://uth.shzxlz.cn

[G14] 数据类 / record
来源：http://izw.kuanghao11.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dck.jinqigufen.top

PHP:  // 用 readonly 属性模拟
来源：http://yep.dashuyun.cn

JS:   // 无内置：普通类或对象字面量
来源：http://guj.redwolf501.top

TS:   type User = { name: string; age: number };
来源：http://cjo.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://lvk.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://dye.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ncg.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://gar.xuanzx.com

[G15] 枚举
来源：http://siu.jinyuanbaomall.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sud.316326.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ugj.nanxuanxn.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mov.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://icb.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://yil.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mac.hesvh.cn

Ruby: Color = %i[red green].freeze
来源：http://gdj.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nzy.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://ctd.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://isw.yj202588.top

PHP:  get_object_vars($obj);
来源：http://llx.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://jfu.wangdashe.top

TS:   Object.entries(obj)
来源：http://wtd.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zhw.ywan-chungtsiang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rbd.zhengqikj.top

Ruby: obj.instance_variables
来源：http://vrf.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://pjm.hesvh.cn

================================================================================
来源：http://mxt.ydzc1.top

H. 异常与错误处理
来源：http://vsc.tianlin.xyz

================================================================================
来源：http://jnu.bjfxy.top

[H01] try / catch 基础
来源：http://qxy.shzxlz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vcj.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tit.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://phg.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://apo.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hkg.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eoi.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mqq.wangdashe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hca.ivvv.top

[H02] finally / ensure 收尾
来源：http://kuq.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://ypk.aizwys.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xyu.ivvv.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wut.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://czr.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://fpq.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://kbw.tanke756.top

Ruby: begin; f; ensure; cleanup; end
来源：http://oof.zhijiandao.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sld.hammf.cn

[H03] 主动抛出异常
来源：http://ovd.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://mhx.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gol.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://luy.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://qan.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://frp.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sch.hammf.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hhw.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bhh.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://dhl.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://cgj.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://kne.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://ifz.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://lju.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://yym.0kj1m.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wri.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://hrw.epnwcf.com

C#:   class MyException : Exception {}
来源：http://ddr.fehbvm.com

[H05] 捕获特定类型
来源：http://vhm.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://sez.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nqb.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://eng.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://zmv.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://ikt.daria6918.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lea.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://kzp.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nke.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://tif.uphjek.com

Py:   value = d.get("k") or default
来源：http://sfa.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mge.hcnkem.com

JS:   obj?.a?.b;  d ?? default
来源：http://jve.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hwf.cashguo.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ybw.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://piu.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://ckn.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://ccd.daria6918.cn

[H07] 断言
来源：http://zcu.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://jty.vehdjk.com

PHP:  assert($x > 0);
来源：http://tyv.fehbvm.com

JS:   console.assert(x > 0);
来源：http://hvq.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://sah.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://hoo.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ywx.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lqy.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://fgp.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://goa.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://rcm.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wum.xziqi.cn

JS:   e.message;  e.stack
来源：http://lth.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rpy.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jui.zhijiandao.cn

Go:   err.Error()
来源：http://onq.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://qsn.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://enz.yuxming.cn

[H09] 带错误码的异常
来源：http://nbk.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jkh.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ndh.cashguo.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wcr.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gxs.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fkt.meibo888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hyy.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://eod.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jsb.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://xfd.hesvh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wzv.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jjq.jqgfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sii.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dsj.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kyf.hesvh.cn

Go:   defer f.Close()
来源：http://dnq.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wlt.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gev.ctjpmb.com

================================================================================
来源：http://gis.jiagoushi.top

I. 正则表达式
来源：http://pxz.havefunace.top

================================================================================
来源：http://fjm.ydzc1.top

[I01] 判断是否匹配
来源：http://lqw.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fvx.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://krb.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://kll.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://rwu.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ygd.yfazqb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dsy.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://hnf.kuanghao11.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://teo.zhengqikj.top

[I02] 提取所有匹配
来源：http://yqk.shzxlz.cn

Py:   re.findall(r"\d+", s)
来源：http://evk.daxiang520.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hqq.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hnh.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://jmr.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uzp.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://obk.wangshuangyany.cn

Ruby: s.scan(/\d+/)
来源：http://qzw.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kby.yj20258.top

[I03] 提取捕获分组
来源：http://aho.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dva.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xkv.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hyp.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cbj.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pyj.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://krm.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://erd.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oah.chenlongwang.top

[I04] 正则替换
来源：http://euc.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sbo.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bmw.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://zpd.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://nvu.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://gfz.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fzo.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uce.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kky.yj202588.top

[I05] 按正则拆分
来源：http://urq.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tne.tarul.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wmb.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://ymv.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://mou.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://wvd.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ijb.jianghu66.top

Ruby: s.split(/\s*,\s*/)
来源：http://tpt.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dnd.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tho.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pxw.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wox.tarul.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ebk.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mop.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cwh.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gku.wangshuangyany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hye.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://was.nwbrower.top

[I07] 忽略大小写与多行模式
来源：http://frt.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ici.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sjk.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eau.ctjpmb.com

TS:   /error/gim
来源：http://tvd.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ogf.tian-w.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ftu.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://qwn.chenlongwang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lia.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://wvw.yanxiufei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gec.cucudq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aqn.snrcjt.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qbc.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pga.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sgc.wangshuangyany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tsk.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://knp.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://frf.jyoumei.cn

================================================================================
来源：http://ekj.sufxvd.cn

J. 日期与时间
来源：http://cse.gaohongyu789.top

================================================================================
来源：http://znc.zhengqikj.top

[J01] 获取当前时间
来源：http://gca.chenlongwang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ehw.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zjm.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://xee.andypj.xyz

TS:   new Date();  Date.now()
来源：http://tvy.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ckf.hfpthk.cn

Go:   time.Now()
来源：http://wjz.hnqzz.top

Ruby: Time.now
来源：http://pxh.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dkt.hcnkem.com

[J02] 格式化输出
来源：http://shd.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qwj.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kfs.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nit.epnwcf.com

TS:   d.toISOString()
来源：http://lmd.gaohongyu789.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dby.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mtb.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xif.9152youxi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gji.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://ced.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jzw.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hie.uphjek.com

JS:   new Date("2024-01-02")
来源：http://mkc.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://zct.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eqp.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aqg.shangyingyoupin.top

Ruby: Date.parse("2024-01-02")
来源：http://hos.chenlongwang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gjx.yfazqb.com

[J04] 时间戳与日期互转
来源：http://kzw.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wfl.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iks.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ffv.tian-w.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oik.shanyushiyangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iqa.fzhhl.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nsr.zhixingplan.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ehf.jlsjyb.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wqe.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://ofu.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://txs.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://bks.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xqp.jqgfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vhs.fengsongda.top

Java: LocalDate.now().plusDays(7)
来源：http://dwa.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aen.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://vrb.svipenyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fzj.gaohongyu789.top

[J06] 计算两时间之差
来源：http://yxl.cheryme.top

Py:   (end - start).total_seconds()
来源：http://fap.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://xvw.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://roo.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pdc.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mcg.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://guu.316326.xyz

Ruby: end - start                 # 返回秒数
来源：http://klh.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://jrf.zdbjq.cn

[J07] 比较两个日期
来源：http://syq.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://pwf.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yto.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://thw.shangyingyoupin.top


<!-- 参考信息 -->