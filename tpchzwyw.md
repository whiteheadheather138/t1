代发 wailian999

Java: interface Shape { double area(); }
来源：http://bef.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://wlg.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mwp.iojbl.cn

C#:   interface IShape { double Area(); }
来源：http://lgd.yj20258888.top

[G10] 访问控制
来源：http://wts.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://onc.pengpengdd.cyou

PHP:  public / protected / private
来源：http://bns.xuanzx.com

JS:   #private 字段；其余公开
来源：http://pea.quarkkingdee.top

TS:   public / protected / private
来源：http://bxs.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://ast.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://awa.ctjpmb.com

Ruby: public / protected / private
来源：http://fjz.ivvv.top

C#:   public / protected / private / internal
来源：http://ygi.tian-w.cn

[G11] getter / setter
来源：http://fdr.aizwys.cn

Py:   @property 与 @x.setter
来源：http://fsr.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vil.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://jmm.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://erd.chenzaomai.com

Java: public String getName() { return name; }
来源：http://wua.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://mce.yueranfly.top

Ruby: attr_accessor :name
来源：http://ogo.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://utq.316326.xyz

[G12] 对象转字符串
来源：http://mwl.gaohongyu789.top

Py:   def __str__(self): return self.name
来源：http://rmq.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ohi.ydjk.org.cn

JS:   toString() { return this.name; }
来源：http://pon.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://msd.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://mbs.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ixa.yongpay.top

Ruby: def to_s; @name; end
来源：http://vpl.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://poo.bbcook.cn

[G13] 判断对象类型
来源：http://kqv.zhengqikj.top

Py:   isinstance(u, User)
来源：http://ssw.wangdashe.top

PHP:  $u instanceof User
来源：http://gnh.jianghu66.top

JS:   u instanceof User
来源：http://svg.yj20258.top

TS:   u instanceof User
来源：http://iud.shangyingyoupin.top

Java: u instanceof User
来源：http://vty.cashguo.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ubl.ybcxt.top

Ruby: u.is_a?(User)
来源：http://nbz.wangdashe.top

C#:   u is User
来源：http://bzf.kuanghao11.cn

[G14] 数据类 / record
来源：http://rya.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pnw.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://fiw.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://ryr.uphjek.com

TS:   type User = { name: string; age: number };
来源：http://cau.vehdjk.com

Java: record User(String name, int age) {}
来源：http://pqt.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://mov.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iru.smart0.xyz

C#:   record User(string Name, int Age);
来源：http://zlt.tianlin.xyz

[G15] 枚举
来源：http://yvw.gogol.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uko.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://txn.yfazqb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jbs.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sia.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://xkj.nanxuanxn.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tsi.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://qsm.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zya.hammf.cn

[G16] 对象转数组 / 字典
来源：http://wrq.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://maf.wangshuangyany.cn

PHP:  get_object_vars($obj);
来源：http://dxz.gotoacloud.top

JS:   Object.entries(obj)
来源：http://kiw.dianchejie.cn

TS:   Object.entries(obj)
来源：http://nyj.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xay.ctjpmb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ttu.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://moj.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://gge.hfpthk.cn

================================================================================
来源：http://vtw.fzhhl.top

H. 异常与错误处理
来源：http://bfs.svipenyu.cn

================================================================================
来源：http://jni.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://ebu.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hqf.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uft.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kqz.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dac.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zbt.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://raq.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gyp.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mck.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://yrd.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://pya.guowangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jhq.zhoulong.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://kvt.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://chd.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bjp.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xbl.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xfi.yonumen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nnt.gogol.net.cn

[H03] 主动抛出异常
来源：http://nbp.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://lnr.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mwm.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://tbn.tanke756.top

TS:   throw new Error("错误信息");
来源：http://irp.quarkkingdee.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lia.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://two.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xka.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://svj.yanxiufei.cn

[H04] 自定义异常类型
来源：http://xon.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://ffm.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bsj.fzhhl.top

JS:   class MyError extends Error {}
来源：http://afk.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://vor.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://thb.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rwn.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://yuh.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://xkg.xylfe.cn

[H05] 捕获特定类型
来源：http://mbx.smart0.xyz

Py:   except ValueError as e:
来源：http://bdl.xinyue.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eeg.cucudq.cn

JS:   if (e instanceof TypeError) {}
来源：http://puf.zhaomingkeji.xyz

TS:   if (e instanceof TypeError) {}
来源：http://dho.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://smw.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xdm.yonumen.top

Ruby: rescue ArgumentError => e
来源：http://npu.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zjq.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://uuc.tian-w.cn

Py:   value = d.get("k") or default
来源：http://yov.yangfankeji.com

PHP:  $v = $d["k"] ?? null;
来源：http://hlo.ivvv.top

JS:   obj?.a?.b;  d ?? default
来源：http://ezl.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vsu.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ibo.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bwu.vehdjk.com

Ruby: d&.dig(:a, :b)
来源：http://jro.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://kaw.wangdashe.top

[H07] 断言
来源：http://gam.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://ntg.cucudq.cn

PHP:  assert($x > 0);
来源：http://cky.cashguo.top

JS:   console.assert(x > 0);
来源：http://tph.bjfxy.top

TS:   console.assert(x > 0);
来源：http://oaq.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://kya.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gcf.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cqe.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://gda.shzxlz.cn

[H08] 获取错误信息与堆栈
来源：http://evr.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://eeb.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pet.meibo888.top

JS:   e.message;  e.stack
来源：http://rop.fktsv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ypy.c1oappe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vvb.xuetiantiany.cn

Go:   err.Error()
来源：http://npi.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://fcm.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://tda.jqgfzy.top

[H09] 带错误码的异常
来源：http://fcr.zycfv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://trs.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://agl.jinghuilouyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mbw.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pio.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cao.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ytk.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://mti.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://lae.0kj1m.cn

[H10] 资源自动释放
来源：http://rkh.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://cjc.xinyue.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jvg.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bjd.jinghuilouyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gps.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zoe.shangyingyoupin.top

Go:   defer f.Close()
来源：http://hed.zhixingplan.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lcm.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yuy.yj20258.top

================================================================================
来源：http://lqq.kuanghao11.cn

I. 正则表达式
来源：http://qao.hywenlv.cn

================================================================================
来源：http://ajp.dashuyun.cn

[I01] 判断是否匹配
来源：http://kir.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xbj.dashuyun.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gtt.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://kgl.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://dol.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ose.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://scg.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://xqd.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zmn.cqqwz.cn

[I02] 提取所有匹配
来源：http://zsc.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://zdd.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gnw.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dps.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://ohq.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lfw.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jbs.shanyushiyangkeji.top

Ruby: s.scan(/\d+/)
来源：http://fzl.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://inu.jinghuilouyu.cn

[I03] 提取捕获分组
来源：http://jsa.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vop.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wil.yangfankeji.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eqw.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mqi.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pxl.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://twv.birdmap.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://azl.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://onu.tian-w.cn

[I04] 正则替换
来源：http://qdn.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://yfh.nanxinkj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dkw.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://kzs.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nkq.dianchejie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dqe.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fmu.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://iad.bjfxy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lod.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://cqp.snrcjt.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lmr.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ufx.zdqjudy.top

JS:   s.split(/\s*,\s*/)
来源：http://wpw.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://msx.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://del.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lnm.zhaomingkeji.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ckp.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rwx.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hgo.wangshuangyany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kwh.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dbh.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uxh.uphjek.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://thy.andypj.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qed.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tzc.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ypm.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tiw.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://qxm.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qpq.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ykh.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zij.cdnleiting.top

TS:   /error/gim
来源：http://wie.sweek.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kow.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tau.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://tva.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vor.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://kbq.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ynq.bbcook.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://run.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://huz.cucudq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vxq.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qpi.xuanzx.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tac.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pri.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ngr.hysaishi.cn

================================================================================
来源：http://znl.c1oappe.top

J. 日期与时间
来源：http://lbr.yueranfly.top

================================================================================
来源：http://cid.guowangkeji.top

[J01] 获取当前时间
来源：http://dzi.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cap.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nwh.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://dch.snrcjt.cn

TS:   new Date();  Date.now()
来源：http://rxi.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qvi.quarkkingdee.top

Go:   time.Now()
来源：http://wyh.vqdsnc.cn

Ruby: Time.now
来源：http://oiq.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mmd.feifeiyinyue.top

[J02] 格式化输出
来源：http://lfi.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://snj.sufxvd.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nnm.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ndj.cashguo.top

TS:   d.toISOString()
来源：http://ogx.hnxiangtu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ril.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uqm.316326.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xfk.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ckq.jiagoushi.top

[J03] 字符串解析为日期
来源：http://tht.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ynx.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hrm.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://lnu.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://szo.xylfe.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lmq.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ylc.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://ygw.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vcd.yuxming.cn

[J04] 时间戳与日期互转
来源：http://jcc.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://usi.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tgs.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zet.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://klb.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tdn.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vmk.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zns.daxiang520.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tov.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://iof.tarul.cn

Py:   now + timedelta(days=7)
来源：http://ihl.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://foy.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eul.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://urk.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://mhh.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lpj.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://ulo.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://mph.jinqigfzy.top

[J06] 计算两时间之差
来源：http://esv.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://dng.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://rxf.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qwp.tianlin.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://adl.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qbg.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://aur.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://mwh.ywan-chungtsiang.top

C#:   (end - start).TotalSeconds
来源：http://air.nwbrower.top

[J07] 比较两个日期
来源：http://vkt.yuanzhike.top

Py:   d1 < d2;  d1 == d2
来源：http://xvh.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rwy.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://fml.vqdsnc.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qxz.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jss.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://odw.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://hti.sysykeji.top


<!-- 参考信息 -->