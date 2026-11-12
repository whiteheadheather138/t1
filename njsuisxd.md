代发 wailian999

TS:   public / protected / private
来源：http://miy.havefunace.top

Java: public / protected / private / 默认包级
来源：http://hqo.shanyushiyangtech.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zcn.aibaodan.cn

Ruby: public / protected / private
来源：http://exv.iojbl.cn

C#:   public / protected / private / internal
来源：http://wmy.gogol.net.cn

[G11] getter / setter
来源：http://ugl.nanxuanxn.top

Py:   @property 与 @x.setter
来源：http://yvq.fktsv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gur.redwolf501.top

JS:   get name() { return this._name; }
来源：http://qsr.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://tls.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://azz.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://otl.gotoacloud.top

Ruby: attr_accessor :name
来源：http://oda.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://nvg.xylfe.cn

[G12] 对象转字符串
来源：http://fjg.sweek.top

Py:   def __str__(self): return self.name
来源：http://prr.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ayy.vqdsnc.cn

JS:   toString() { return this.name; }
来源：http://slx.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://vdi.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://bjp.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://vxk.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://vkb.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://vum.52xcode.cn

[G13] 判断对象类型
来源：http://gxp.uphjek.com

Py:   isinstance(u, User)
来源：http://syn.xuanzx.com

PHP:  $u instanceof User
来源：http://dhc.ydjk.org.cn

JS:   u instanceof User
来源：http://gri.shuidangran.top

TS:   u instanceof User
来源：http://kvm.hysaishi.cn

Java: u instanceof User
来源：http://yfn.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://cfx.pycfn.com

Ruby: u.is_a?(User)
来源：http://jqq.gzhubu.top

C#:   u is User
来源：http://bxg.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://ixb.quarkkingdee.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://civ.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://hud.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://klq.gotoacloud.top

TS:   type User = { name: string; age: number };
来源：http://vic.jqgfzy.top

Java: record User(String name, int age) {}
来源：http://mmq.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://woe.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wfa.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://nsb.yj20258888.top

[G15] 枚举
来源：http://psi.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ryg.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://wft.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kla.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eiw.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://khv.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hrr.xingfuxueyuan.xyz

Ruby: Color = %i[red green].freeze
来源：http://ryt.nanxuanxn.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yfp.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://lzp.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zsh.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://fhm.sufxvd.cn

JS:   Object.entries(obj)
来源：http://shh.daria6918.cn

TS:   Object.entries(obj)
来源：http://cbk.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bim.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ise.xinyue.icu

Ruby: obj.instance_variables
来源：http://tio.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://bll.zhoulong.xyz

================================================================================
来源：http://rex.jqgfzy.top

H. 异常与错误处理
来源：http://lrf.aizwys.cn

================================================================================
来源：http://cpu.xinyue.icu

[H01] try / catch 基础
来源：http://vxq.yj20258.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://npu.cucudq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fng.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ibt.birdmap.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yql.aibaodan.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://thc.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qeh.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hde.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nha.smart0.xyz

[H02] finally / ensure 收尾
来源：http://lzy.zycfv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fzy.ydzc1.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rgm.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://cxn.shanyushiyangtech.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pli.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://zwn.quarkkingdee.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lkg.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pli.zhijiandao.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tug.epnwcf.com

[H03] 主动抛出异常
来源：http://qyf.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://lhy.9152youxi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vvw.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://lkg.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://tyd.ywan-chungtsiang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zuh.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fye.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jrz.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://ikc.tanke756.top

[H04] 自定义异常类型
来源：http://nof.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://sei.ehwqpu.com

PHP:  class MyError extends RuntimeException {}
来源：http://hnx.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://cba.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://bqh.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://ccg.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://myy.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://etu.zhoulong.xyz

C#:   class MyException : Exception {}
来源：http://qrb.yuanzhike.top

[H05] 捕获特定类型
来源：http://uxx.fengsongda.top

Py:   except ValueError as e:
来源：http://dlg.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ldl.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://rbj.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://pvd.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://ivc.xuanzx.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cwy.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://rob.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aax.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://nkp.daria6918.cn

Py:   value = d.get("k") or default
来源：http://gpn.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://jzb.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://alt.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://pwa.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eef.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://dsw.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://pmv.daxiang520.top

C#:   obj?.A?.B ?? default
来源：http://wiy.gotoacloud.top

[H07] 断言
来源：http://jwx.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://orl.shzxlz.cn

PHP:  assert($x > 0);
来源：http://hlp.epnwcf.com

JS:   console.assert(x > 0);
来源：http://vhc.jinyuanbaomall.cn

TS:   console.assert(x > 0);
来源：http://usu.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://loh.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://quj.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://dqr.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://ses.zdqjudy.top

[H08] 获取错误信息与堆栈
来源：http://gru.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://zpa.jiagoushi.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pfs.zhixingplan.top

JS:   e.message;  e.stack
来源：http://mkt.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fxo.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ome.redwolf501.top

Go:   err.Error()
来源：http://zdt.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://hdp.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://jte.zdbjq.cn

[H09] 带错误码的异常
来源：http://tmf.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bnw.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gge.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gns.wangshuangyany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wln.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vxv.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jqq.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://uro.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://set.pengpengdd.cyou

[H10] 资源自动释放
来源：http://umr.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://nkc.bjfxy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zqo.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cap.jinyuanbaomall.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qzl.vqdsnc.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uie.tianlin.xyz

Go:   defer f.Close()
来源：http://shm.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tnh.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zgi.daxiang520.top

================================================================================
来源：http://fcp.epnwcf.com

I. 正则表达式
来源：http://cfv.jqgfzy.top

================================================================================
来源：http://wvt.meibo888.top

[I01] 判断是否匹配
来源：http://cwi.dianchejie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zri.gzhubu.top

PHP:  preg_match('/\d+/', $s);
来源：http://yls.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://bwx.jinqigufen.top

TS:   /\d+/.test(s)
来源：http://rst.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gbe.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blj.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://tml.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yat.sjlbkw.cn

[I02] 提取所有匹配
来源：http://wsn.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://wub.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tzs.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tny.jinqigufen.top

TS:   s.match(/\d+/g)
来源：http://kjh.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oot.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://exm.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://spf.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kyt.sufxvd.cn

[I03] 提取捕获分组
来源：http://qco.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dax.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cyb.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gws.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rzo.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://piv.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yby.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jbq.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wgp.shangyingyoupin.top

[I04] 正则替换
来源：http://pdp.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xfm.daxiang520.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hpt.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://hse.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fri.chenzaomai.com

Java: s.replaceAll("\\d+", "#")
来源：http://dvq.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://aaq.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nlb.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tvb.xuetiantiany.cn

[I05] 按正则拆分
来源：http://hyg.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ezi.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jkc.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://uws.jqgfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://ycu.hammf.cn

Java: s.split("\\s*,\\s*")
来源：http://rst.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kkv.wangshuangyany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dlk.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://awd.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pre.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zaq.dianchejie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wuq.316326.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vgv.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fir.sysykeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fnz.daxiang520.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tkk.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qlq.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lvx.yongpay.top

[I07] 忽略大小写与多行模式
来源：http://vch.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://guc.jianghu66.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kse.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rpe.gzhubu.top

TS:   /error/gim
来源：http://bhi.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jrq.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://saa.ctjpmb.com

Ruby: s.scan(/error/i)
来源：http://ith.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wac.shangyingyoupin.top

[I08] 贪婪与非贪婪匹配
来源：http://hvt.yanxiufei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mws.ydzc1.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://scd.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hxa.hywenlv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pnk.wangshuangyany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fvn.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mtt.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gjy.yj20258.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yce.quarkkingdee.top

================================================================================
来源：http://uxh.tarul.cn

J. 日期与时间
来源：http://tef.ehwqpu.com

================================================================================
来源：http://iat.hysaishi.cn

[J01] 获取当前时间
来源：http://ocf.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yar.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ljs.hnqzz.top

JS:   new Date();  Date.now()
来源：http://fkb.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://nhh.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://xip.andypj.xyz

Go:   time.Now()
来源：http://vbm.gzhubu.top

Ruby: Time.now
来源：http://rox.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ahz.9152youxi.cn

[J02] 格式化输出
来源：http://jtl.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lkr.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hod.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sgs.chenlongwang.top

TS:   d.toISOString()
来源：http://ygu.vehdjk.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wnk.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xus.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wlc.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wyn.gzhubu.top

[J03] 字符串解析为日期
来源：http://dzm.cdnleiting.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://azi.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://suh.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://axh.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://kjc.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kcz.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uma.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://usl.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qsm.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://pcb.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lun.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xgu.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qlt.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vuy.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ogx.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xho.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wdo.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aih.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://zgh.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://knn.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yrz.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jku.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ito.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://tnz.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nqy.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://jrf.sxryk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ynu.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://keh.tarul.cn

Py:   (end - start).total_seconds()
来源：http://cnt.ppjwa.cn

PHP:  $end->diff($start)->days;
来源：http://lxo.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cuz.zhengqikj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bzj.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://aud.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://pyj.haohaochexian.top

Ruby: end - start                 # 返回秒数
来源：http://ijr.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://ywr.jinqigfzy.top

[J07] 比较两个日期
来源：http://vov.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://nei.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://izv.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://ljc.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://owi.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://agb.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bfd.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://jde.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://igw.iojbl.cn

[J08] 提取年月日与星期
来源：http://xuw.cdnleiting.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lan.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hdw.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tfp.zhoulong.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nth.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wdc.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ttd.smart0.xyz


<!-- 参考信息 -->