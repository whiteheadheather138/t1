代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://qvb.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zru.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tmp.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://qlk.chenjidiqi.icu

Java: interface Shape { double area(); }
来源：http://ils.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://vom.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wbd.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://ggo.nwbrower.top

[G10] 访问控制
来源：http://cjz.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://yjx.yj20258.top

PHP:  public / protected / private
来源：http://gev.iojbl.cn

JS:   #private 字段；其余公开
来源：http://lat.zdqjudy.top

TS:   public / protected / private
来源：http://oxg.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://box.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://bkv.tarul.cn

Ruby: public / protected / private
来源：http://vms.cqqwz.cn

C#:   public / protected / private / internal
来源：http://elc.xziqi.cn

[G11] getter / setter
来源：http://dsg.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://ywl.c1oappe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dtx.yuxming.cn

JS:   get name() { return this._name; }
来源：http://rur.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://tyl.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://ttp.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wbj.havefunace.top

Ruby: attr_accessor :name
来源：http://dje.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://kfq.yj20258.top

[G12] 对象转字符串
来源：http://ryo.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://zyl.sufxvd.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ucd.yonumen.top

JS:   toString() { return this.name; }
来源：http://pas.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://xle.vehdjk.com

Java: @Override public String toString() { return name; }
来源：http://kev.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://bih.fktsv.cn

Ruby: def to_s; @name; end
来源：http://isf.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://znd.gzhubu.top

[G13] 判断对象类型
来源：http://uea.havefunace.top

Py:   isinstance(u, User)
来源：http://kvc.xziqi.cn

PHP:  $u instanceof User
来源：http://wea.yfazqb.com

JS:   u instanceof User
来源：http://lnn.zhongyouzk.top

TS:   u instanceof User
来源：http://wev.ydzc1.top

Java: u instanceof User
来源：http://ozq.ydjk.org.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iep.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://tfi.kuanghao11.cn

C#:   u is User
来源：http://bvd.cdnleiting.top

[G14] 数据类 / record
来源：http://wsa.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wun.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://cvy.hfpthk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lns.tanke756.top

TS:   type User = { name: string; age: number };
来源：http://vgm.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://kgn.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://scb.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://str.zdbjq.cn

C#:   record User(string Name, int Age);
来源：http://wyx.iojbl.cn

[G15] 枚举
来源：http://gxh.iojbl.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ikd.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gql.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://phu.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yba.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://hic.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lrb.feifeiyinyue.top

Ruby: Color = %i[red green].freeze
来源：http://poo.aibaodan.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mqg.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://vfq.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fbc.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://efa.jiagoushi.top

JS:   Object.entries(obj)
来源：http://dcp.yj20258888.top

TS:   Object.entries(obj)
来源：http://lbx.52xcode.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tjd.tianlin.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://hcc.cheryme.top

Ruby: obj.instance_variables
来源：http://lhl.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://yiy.zdqjudy.top

================================================================================
来源：http://klh.ydzc1.top

H. 异常与错误处理
来源：http://ftc.gzhubu.top

================================================================================
来源：http://tqo.jinqigfzy.top

[H01] try / catch 基础
来源：http://wgu.jlsjyb.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vru.zhixingplan.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pzz.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ikc.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cqe.ydjk.org.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qer.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zrz.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qnc.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kwy.zycfv.cn

[H02] finally / ensure 收尾
来源：http://zbz.ybcxt.top

Py:   try: f()⏎finally: cleanup()
来源：http://xhn.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://raz.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://nna.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://xwp.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zzl.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ozl.zhijiandao.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://khj.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bxv.yuxming.cn

[H03] 主动抛出异常
来源：http://nww.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://mzj.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vok.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://pvl.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://pfr.gotoacloud.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://eua.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://upu.guannengcc.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dzs.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://fss.jiagoushi.top

[H04] 自定义异常类型
来源：http://alp.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://muu.fengsongda.top

PHP:  class MyError extends RuntimeException {}
来源：http://jza.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://ywi.bbcook.cn

TS:   class MyError extends Error {}
来源：http://mfu.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://zlf.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gnc.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://wkn.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://ueg.jinqigfzy.top

[H05] 捕获特定类型
来源：http://qmq.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://wak.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ewh.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://ucs.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://gis.meibo888.top

Java: catch (IOException | SQLException e) {}
来源：http://afk.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hie.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://nlg.hcnkem.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://glp.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://viv.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://ygs.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://vvd.shangyingyoupin.top

JS:   obj?.a?.b;  d ?? default
来源：http://ltn.daria6918.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lzz.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jwl.sjlbkw.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vvu.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://zav.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://mnn.jinqigufen.top

[H07] 断言
来源：http://qyy.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://xld.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://dcq.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://jxk.fengsongda.top

TS:   console.assert(x > 0);
来源：http://gts.jqgufenzy.top

Java: assert x > 0 : "必须为正";
来源：http://cxu.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sib.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wmr.c1oappe.top

C#:   Debug.Assert(x > 0);
来源：http://ufd.jinqigfzy.top

[H08] 获取错误信息与堆栈
来源：http://xnm.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://euu.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zqm.52xcode.cn

JS:   e.message;  e.stack
来源：http://lpa.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kfr.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nwq.jianghu66.top

Go:   err.Error()
来源：http://xok.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://anz.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://hgk.tarul.cn

[H09] 带错误码的异常
来源：http://oyc.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hmf.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://coc.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pmz.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fen.hesvh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vxx.daxiang520.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dlu.yj202588.top

Ruby: raise MyError.new("fail", 500)
来源：http://wvc.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pfc.iojbl.cn

[H10] 资源自动释放
来源：http://ytk.smart0.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://mcu.yuxming.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sli.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vxh.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rcn.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ezy.chenjidiqi.icu

Go:   defer f.Close()
来源：http://uby.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zlu.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gjz.hesvh.cn

================================================================================
来源：http://phu.meibo888.top

I. 正则表达式
来源：http://gfw.yj20258888.top

================================================================================
来源：http://nib.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://lib.yfazqb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://stq.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rqj.epnwcf.com

JS:   /\d+/.test(s)
来源：http://lhm.yvedp.cn

TS:   /\d+/.test(s)
来源：http://faz.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mwq.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ctv.316326.xyz

Ruby: s.match?(/\d+/)
来源：http://oxa.fanxiaobao.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tni.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://gvg.dashuyun.cn

Py:   re.findall(r"\d+", s)
来源：http://aqa.jinqigfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mqe.uphjek.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nvn.guowangkeji.top

TS:   s.match(/\d+/g)
来源：http://daf.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xvy.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mog.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://gll.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vds.nanxuanxn.top

[I03] 提取捕获分组
来源：http://edp.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ywb.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hrb.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wou.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bjd.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gby.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ybs.snrcjt.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gym.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dwd.gotoacloud.top

[I04] 正则替换
来源：http://ipq.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zjf.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ezr.xinyue.icu

JS:   s.replace(/\d+/g, "#")
来源：http://rrs.aibaodan.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ymm.shzxlz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fza.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uym.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rdh.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yya.nanxinkj.top

[I05] 按正则拆分
来源：http://qvq.gogol.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ovq.birdmap.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lpt.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://gyk.316326.xyz

TS:   s.split(/\s*,\s*/)
来源：http://msi.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://oeg.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tna.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ans.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kjx.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dtu.nanxinkj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kzu.hammf.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aby.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zte.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gtt.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fzk.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ydk.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rhg.xylfe.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xph.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://xbc.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://afk.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ytu.nanxinkj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://and.yj20258888.top

TS:   /error/gim
来源：http://tqn.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qhw.gzhubu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://shg.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://byh.yuanzhike.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rbn.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://mqv.xylfe.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xby.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ukb.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jtr.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mtx.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xqz.tanke756.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oey.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gpl.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cce.uphjek.com

================================================================================
来源：http://ela.redwolf501.top

J. 日期与时间
来源：http://xxb.ehwqpu.com

================================================================================
来源：http://rkt.tarul.cn

[J01] 获取当前时间
来源：http://zqg.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://evh.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zmb.yfazqb.com

JS:   new Date();  Date.now()
来源：http://jes.yuxming.cn

TS:   new Date();  Date.now()
来源：http://fod.yj202588.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qlb.hfpthk.cn

Go:   time.Now()
来源：http://uis.daria6918.cn

Ruby: Time.now
来源：http://koo.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iui.ehwqpu.com

[J02] 格式化输出
来源：http://kvv.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mpo.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yzl.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fls.vehdjk.com

TS:   d.toISOString()
来源：http://dhu.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://etp.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nea.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ywz.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ejs.sxryk.cn

[J03] 字符串解析为日期
来源：http://qpg.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wpg.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jsi.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://qbd.xuanzx.com

TS:   new Date("2024-01-02")
来源：http://nhq.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rfg.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xev.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://oni.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ugb.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://evy.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qto.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vle.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jvl.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ife.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qph.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wgo.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pvc.jinqigfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ixp.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://clf.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://bvv.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://kta.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mnk.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ryo.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://dil.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://toq.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://qjo.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://frk.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://rjx.havefunace.top

Py:   (end - start).total_seconds()
来源：http://inb.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://bca.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kat.gotoacloud.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ilv.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://ugg.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://vqj.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://ayj.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://obo.jianghu66.top

[J07] 比较两个日期
来源：http://dam.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://zsw.shangyingyoupin.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ebe.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lvh.yueranfly.top


<!-- 参考信息 -->