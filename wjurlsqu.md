代发 wailian999

[G10] 访问控制
来源：http://sgb.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://nks.feifeiyinyue.top

PHP:  public / protected / private
来源：http://ewu.uphjek.com

JS:   #private 字段；其余公开
来源：http://reh.nwbrower.top

TS:   public / protected / private
来源：http://gdu.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://kdq.haohaochexian.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mgp.uphjek.com

Ruby: public / protected / private
来源：http://gqi.gotoacloud.top

C#:   public / protected / private / internal
来源：http://udp.cdnleiting.top

[G11] getter / setter
来源：http://cfx.xylfe.cn

Py:   @property 与 @x.setter
来源：http://aot.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://bwg.tian-w.cn

JS:   get name() { return this._name; }
来源：http://wzu.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://aiq.vehdjk.com

Java: public String getName() { return name; }
来源：http://nhe.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://obe.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://qat.hesvh.cn

C#:   public string Name { get; set; }
来源：http://wrn.cashguo.top

[G12] 对象转字符串
来源：http://pgv.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://hqs.sufxvd.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qrg.ydzc1.top

JS:   toString() { return this.name; }
来源：http://faz.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://rhw.smart0.xyz

Java: @Override public String toString() { return name; }
来源：http://pid.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://ebd.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://rbz.shanyushiyangtech.top

C#:   public override string ToString() => Name;
来源：http://hvp.9152youxi.cn

[G13] 判断对象类型
来源：http://ynk.hongshengwenyu.top

Py:   isinstance(u, User)
来源：http://zhu.316326.xyz

PHP:  $u instanceof User
来源：http://rvu.yj20258.top

JS:   u instanceof User
来源：http://aop.tianlin.xyz

TS:   u instanceof User
来源：http://ono.0kj1m.cn

Java: u instanceof User
来源：http://wot.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dii.yongpay.top

Ruby: u.is_a?(User)
来源：http://mxr.wangshuangyany.cn

C#:   u is User
来源：http://kmt.xylfe.cn

[G14] 数据类 / record
来源：http://vhr.gotoacloud.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jpm.9152youxi.cn

PHP:  // 用 readonly 属性模拟
来源：http://cin.mhx1999.top

JS:   // 无内置：普通类或对象字面量
来源：http://aye.chenlongwang.top

TS:   type User = { name: string; age: number };
来源：http://xvq.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://lcu.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://zvq.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zdl.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://anh.c1oappe.top

[G15] 枚举
来源：http://jrn.ppjwa.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bhh.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gdq.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pjh.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wcn.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://ztz.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xbr.iojbl.cn

Ruby: Color = %i[red green].freeze
来源：http://mnw.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wtz.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://xpu.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wwx.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://rrj.chenzaomai.com

JS:   Object.entries(obj)
来源：http://mge.zhengqikj.top

TS:   Object.entries(obj)
来源：http://mha.vqdsnc.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oqc.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lrn.hcnkem.com

Ruby: obj.instance_variables
来源：http://cxc.zhaomingkeji.xyz

C#:   // 用反射或 System.Text.Json
来源：http://mwf.cucudq.cn

================================================================================
来源：http://qbs.yfazqb.com

H. 异常与错误处理
来源：http://ctt.zhixingplan.top

================================================================================
来源：http://nzq.cheryme.top

[H01] try / catch 基础
来源：http://hzg.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yvl.bjfxy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://olr.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kxl.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wmb.shuidangran.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uet.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ani.fanxiaobao.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sae.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://avl.zycfv.cn

[H02] finally / ensure 收尾
来源：http://hyu.svipenyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://blp.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gfb.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tdp.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://mzd.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://snc.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ahd.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eig.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xwh.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://zuy.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://ykb.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jqk.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://rnr.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://dft.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tkp.ybcxt.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ptu.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bdj.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xco.hfpthk.cn

[H04] 自定义异常类型
来源：http://grp.pycfn.com

Py:   class MyError(Exception): pass
来源：http://qnq.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tdo.andypj.xyz

JS:   class MyError extends Error {}
来源：http://eob.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://epg.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://ukq.chenjidiqi.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wro.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://psm.smart0.xyz

C#:   class MyException : Exception {}
来源：http://tei.shuidangran.top

[H05] 捕获特定类型
来源：http://mke.daria6918.cn

Py:   except ValueError as e:
来源：http://sme.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dbg.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://bkb.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://mhh.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://etg.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ouw.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://grv.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://myx.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://fjw.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://dmb.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://bfx.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://mtr.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://umv.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://spv.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://drp.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://zeb.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://ean.yanxiufei.cn

[H07] 断言
来源：http://fwm.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://ghp.sysykeji.top

PHP:  assert($x > 0);
来源：http://qcy.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://imr.jinyuanbaomall.cn

TS:   console.assert(x > 0);
来源：http://pkl.zdbjq.cn

Java: assert x > 0 : "必须为正";
来源：http://irj.yj202588.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wfu.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://hzq.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://qxc.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://pnq.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://rzu.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oup.mhx1999.top

JS:   e.message;  e.stack
来源：http://ueo.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ueh.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ovd.yvedp.cn

Go:   err.Error()
来源：http://dhm.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://vdb.meibo888.top

C#:   e.Message;  e.StackTrace
来源：http://ojf.chenlongwang.top

[H09] 带错误码的异常
来源：http://hoj.jqgfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rdq.hywenlv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kjw.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ppi.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jbu.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://skb.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://opu.zdbjq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vnj.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://roz.shuidangran.top

[H10] 资源自动释放
来源：http://fff.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wzi.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://khm.zhijiandao.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lou.ppjwa.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://coj.52xcode.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bzz.xuanzx.com

Go:   defer f.Close()
来源：http://yte.cqqwz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://csg.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mlt.birdmap.top

================================================================================
来源：http://kcg.bjfxy.top

I. 正则表达式
来源：http://vbj.zdbjq.cn

================================================================================
来源：http://edn.sjlbkw.cn

[I01] 判断是否匹配
来源：http://hov.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ajj.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://dmg.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://ost.chenzaomai.com

TS:   /\d+/.test(s)
来源：http://cet.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pzv.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nac.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://vho.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://evw.jinghuilouyu.cn

[I02] 提取所有匹配
来源：http://hmr.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://dua.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ylb.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://leq.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://piz.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bfi.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bdp.redwolf501.top

Ruby: s.scan(/\d+/)
来源：http://efk.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mes.gaohongyu789.top

[I03] 提取捕获分组
来源：http://vyv.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ibq.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jeg.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eas.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tkx.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cla.hnxiangtu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hia.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jiv.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rpu.yj20258888.top

[I04] 正则替换
来源：http://hla.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pjx.snrcjt.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lob.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ajk.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://ffb.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mhb.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wco.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://efa.gotoacloud.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kjx.gaohongyu789.top

[I05] 按正则拆分
来源：http://xsp.fanxiaobao.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://nld.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vfg.daxiang520.top

JS:   s.split(/\s*,\s*/)
来源：http://wqm.guannengcc.top

TS:   s.split(/\s*,\s*/)
来源：http://oip.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://skm.chenzaomai.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://drq.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://bpm.hcnkem.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lrz.svipenyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://exm.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vmi.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fmb.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cip.birdmap.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jpg.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vcs.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lpv.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ycg.andypj.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zqb.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://lrx.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yit.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qtb.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ipc.fanxiaobao.xyz

TS:   /error/gim
来源：http://voj.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://agp.zhijiandao.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jgk.fktsv.cn

Ruby: s.scan(/error/i)
来源：http://ymg.zhoulong.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://atr.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://nmr.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gmr.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lzv.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://twt.cdnleiting.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tvt.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tpr.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://epv.yonumen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zeo.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ddr.nanxuanxn.top

================================================================================
来源：http://gsa.feifeiyinyue.top

J. 日期与时间
来源：http://sjx.bbcook.cn

================================================================================
来源：http://szt.zhengqikj.top

[J01] 获取当前时间
来源：http://gvc.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eks.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cku.tarul.cn

JS:   new Date();  Date.now()
来源：http://hep.bbcook.cn

TS:   new Date();  Date.now()
来源：http://vib.iojbl.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://aph.hcnkem.com

Go:   time.Now()
来源：http://nqq.fanxiaobao.xyz

Ruby: Time.now
来源：http://sdh.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ksj.yfazqb.com

[J02] 格式化输出
来源：http://poh.gaohongyu789.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ejm.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uye.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://onj.316326.xyz

TS:   d.toISOString()
来源：http://yzg.iojbl.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kmg.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rzj.aibaodan.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://key.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yqv.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://spv.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://myn.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lph.epnwcf.com

JS:   new Date("2024-01-02")
来源：http://cxy.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://wwf.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://vkw.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ktl.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://dmu.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pzl.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://vqa.sweek.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qtv.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://onf.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://czw.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ero.xinyue.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pmm.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kji.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tns.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cqn.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://rzd.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://avq.quarkkingdee.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fak.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bbo.smart0.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gzu.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://rlg.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cpm.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://vlj.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://eph.ehwqpu.com

[J06] 计算两时间之差
来源：http://dgk.kuanghao11.cn

Py:   (end - start).total_seconds()
来源：http://kud.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://ckp.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kjm.xziqi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gpx.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mxl.hysaishi.cn

Go:   end.Sub(start).Hours()
来源：http://dki.smart0.xyz

Ruby: end - start                 # 返回秒数
来源：http://zhk.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://oaa.ybcxt.top

[J07] 比较两个日期
来源：http://xwm.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://chk.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iwj.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://awa.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://vbo.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jmj.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tdf.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vyh.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://eyk.hammf.cn

[J08] 提取年月日与星期
来源：http://yyx.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zov.gotoacloud.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vjs.jlsjyb.cn


<!-- 参考信息 -->