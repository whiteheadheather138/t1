代发 wailian999

[Q76] 按天统计
来源：http://uuc.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zrw.jinqigufen.top

[Q77] 时间加减
来源：http://bfh.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fep.sxryk.cn

[Q78] 当前时间
来源：http://upl.chenlongwang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mwl.sxryk.cn

[Q79] 字符串拼接
来源：http://gcr.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nay.ydzc1.top

[Q80] 字符串截取
来源：http://kki.zhiwuduotai.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sey.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://qys.ctjpmb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://znq.chenzaomai.com

[Q82] 字符长度与字节长度
来源：http://ecx.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xty.zhengqikj.top

[Q83] 大小写转换
来源：http://iqd.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jio.smart0.xyz

[Q84] 去除首尾空格
来源：http://mhq.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://uzg.tanke756.top

[Q85] 数值取整
来源：http://wdo.fengsongda.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://per.hysaishi.cn

[Q86] 读取 JSON 字段
来源：http://avb.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ees.52xcode.cn

[Q87] JSON 字段做条件
来源：http://vla.zhongyouzk.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://spz.zhijiandao.cn

[Q88] 行转列（条件聚合）
来源：http://xpe.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://epr.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ekr.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://mag.jiagoushi.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pqa.gaohongyu789.top

[Q90] 生成序号列
来源：http://izu.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ays.feifeiyinyue.top

================================================================================
来源：http://ltw.jqgfzy.top

R. Bash 专题
来源：http://hji.yongpay.top

================================================================================
来源：http://pxt.yj20258888.top

[R01] shebang 与严格模式
来源：http://new.gogol.net.cn

#!/usr/bin/env bash
来源：http://lnr.yanxiufei.cn

set -euo pipefail
来源：http://iau.xuanzx.com

[R02] 变量赋值与使用
来源：http://bsm.daria6918.cn

name="Tom"; echo "$name"
来源：http://qiz.xuetiantiany.cn

[R03] 只读变量
来源：http://gis.shanyushiyangtech.top

readonly PI=3.14
来源：http://uqk.xuanzx.com

[R04] 位置参数
来源：http://sms.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dvt.yangfankeji.com

[R05] 参数默认值
来源：http://cva.yonumen.top

name="${1:-default}"
来源：http://nfa.sweek.top

[R06] 判断命令是否存在
来源：http://xdv.ehwqpu.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://srd.haohaochexian.top

[R07] if 判断文件
来源：http://gmo.daria6918.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qnz.bjfxy.top

[R08] 数值比较
来源：http://ire.zhongyouzk.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yhi.zhijiandao.cn

[R09] 字符串比较
来源：http://owr.shanyushiyangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://her.andypj.xyz

[R10] 正则匹配
来源：http://zcy.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qak.jinyuanbaomall.cn

[R11] case 多分支
来源：http://tbv.quarkkingdee.top

case "$1" in
来源：http://bnd.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://qag.zdqjudy.top

stop)  echo "停止" ;;
来源：http://viy.yj202588.top

*)     echo "未知命令" ;;
来源：http://atp.ivvv.top

esac
来源：http://ryi.yuanzhike.top

[R12] for 遍历文件
来源：http://ffa.nanxuanxn.top

for f in *.txt; do echo "$f"; done
来源：http://nao.cqqwz.cn

[R13] for 计数循环
来源：http://utq.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://wms.epnwcf.com

[R14] C 风格 for
来源：http://hew.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qpy.fehbvm.com

[R15] while 逐行读文件
来源：http://ans.kuanghao11.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cnh.snrcjt.cn

[R16] until 等待条件
来源：http://mnj.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tjl.tianlin.xyz

[R17] 数组定义与取值
来源：http://vfv.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://avc.fengsongda.top

[R18] 遍历数组
来源：http://ijh.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ovq.9152youxi.cn

[R19] 数组长度
来源：http://nvq.guannengcc.top

echo "${#arr[@]}"
来源：http://pho.xziqi.cn

[R20] 关联数组（字典）
来源：http://kzr.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lst.316326.xyz

[R21] 字符串长度
来源：http://vyy.xziqi.cn

echo "${#s}"
来源：http://aax.kuanghao11.cn

[R22] 截取子串
来源：http://iwp.sweek.top

echo "${s:0:5}"
来源：http://pyk.yj20258888.top

[R23] 字符串替换
来源：http://hyf.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fli.yangfankeji.com

[R24] 大小写转换
来源：http://edc.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://lez.hnxiangtu.top

[R25] 去后缀 / 去前缀
来源：http://utp.guowangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gig.chenjidiqi.icu

[R26] 命令替换
来源：http://ngt.gotoacloud.top

now=$(date +%F); echo "$now"
来源：http://vsh.cashguo.top

[R27] 算术展开
来源：http://vfc.tarul.cn

echo $((1 + 2 * 3))
来源：http://qpp.shangyingyoupin.top

[R28] 浮点运算
来源：http://ukl.chenlongwang.top

echo "scale=2; 10/3" | bc
来源：http://dup.zhoulong.xyz

[R29] 定义函数
来源：http://sjj.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kob.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://zjh.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://lyd.tarul.cn

[R31] 局部变量
来源：http://jtp.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://xtu.yuanzhike.top

[R32] 参数个数校验
来源：http://afp.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lbc.fanxiaobao.xyz

[R33] 捕获错误并提示行号
来源：http://syo.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://epi.jinqigufen.top

[R34] 退出时清理
来源：http://vax.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://opa.aibaodan.cn

[R35] 后台执行并等待
来源：http://svs.havefunace.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hhj.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://zbr.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hqy.nanxinkj.top

[R37] 把输出赋给变量
来源：http://yok.zhengqikj.top

files=$(ls -1)
来源：http://xuh.xuanzx.com

[R38] 管道串联
来源：http://zdr.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://ena.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://nbo.yj20258.top

cmd > out.log 2>&1
来源：http://yix.52xcode.cn

[R40] 追加写日志
来源：http://rhd.gzhubu.top

echo "log" >> out.log
来源：http://hfl.9152youxi.cn

[R41] 丢弃输出
来源：http://pth.nwbrower.top

cmd >/dev/null 2>&1
来源：http://kwo.sxryk.cn

[R42] 输入重定向
来源：http://rrq.xylfe.cn

wc -l < a.txt
来源：http://wdk.zhongyouzk.top

[R43] 按名字查找文件
来源：http://qmc.jyoumei.cn

find . -name "*.log" -type f
来源：http://csq.yvedp.cn

[R44] 按修改时间查找
来源：http://wdp.tianlin.xyz

find . -mtime -7 -type f
来源：http://jcu.hesvh.cn

[R45] 批量删除
来源：http://xln.jianghu66.top

find . -name "*.tmp" -delete
来源：http://xxf.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://jbx.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rql.havefunace.top

[R47] sed 单行替换
来源：http://puc.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xez.yanxiufei.cn

[R48] awk 取指定列
来源：http://ivv.nwbrower.top

awk '{print $1, $3}' a.txt
来源：http://umv.yj202588.top

[R49] awk 带条件
来源：http://ujg.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://epi.yongpay.top

[R50] awk 求和
来源：http://ztq.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://wzk.ybcxt.top

[R51] 排序去重取前几
来源：http://qye.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nky.bbcook.cn

[R52] 统计行数
来源：http://eky.dashuyun.cn

wc -l a.txt
来源：http://rqs.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://xif.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://npg.hnxiangtu.top

[R54] 比较两个文件
来源：http://ndt.sweek.top

diff a.txt b.txt
来源：http://rni.xylfe.cn

[R55] 压缩与解压
来源：http://ypl.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jqz.guowangkeji.top

[R56] 远程拷贝
来源：http://lsp.hongshengwenyu.top

scp file user@host:/path/
来源：http://zkd.zhongyouzk.top

[R57] 远程执行命令
来源：http://bst.jqgfzy.top

ssh user@host 'uptime'
来源：http://kcx.jyoumei.cn

[R58] 下载文件
来源：http://ots.52xcode.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qfd.redwolf501.top

[R59] 发 POST JSON
来源：http://rol.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pca.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://ykj.ydzc1.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xfv.chenzaomai.com

[R61] 磁盘占用
来源：http://agg.tarul.cn

df -h;  du -sh *
来源：http://dvk.ppjwa.cn

[R62] 找最占空间的文件
来源：http://dpf.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://trf.zhijiandao.cn

[R63] 内存与进程
来源：http://clz.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://kpf.tianlin.xyz

[R64] 结束进程
来源：http://slt.feifeiyinyue.top

kill -9 $(pgrep -f app.py)
来源：http://ndc.tanke756.top

[R65] 查看端口占用
来源：http://wde.hammf.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mfv.hnqzz.top

[R66] 定时任务
来源：http://nvr.vehdjk.com

crontab -e;  crontab -l
来源：http://jmw.zhongyouzk.top

[R67] 生成随机十六进制串
来源：http://yjc.zhoulong.xyz

openssl rand -hex 16
来源：http://kga.tian-w.cn

[R68] 计算文件校验值
来源：http://ymq.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://acz.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://viu.gzhubu.top

head -c 16 /dev/urandom | base64
来源：http://wfw.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://llj.jianghu66.top

date +%s;  date -d @1700000000
来源：http://crg.316326.xyz

[R71] 日期格式化
来源：http://aps.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lcm.zycfv.cn

[R72] 等待端口就绪
来源：http://dot.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lye.fehbvm.com

[R73] 分割大日志
来源：http://qjh.dianchejie.cn

split -l 1000 big.log part_
来源：http://cml.fengsongda.top

[R74] 批量重命名
来源：http://qdg.yuxming.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yqi.uphjek.com

[R75] 导出环境变量
来源：http://gqd.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://kwc.nanxinkj.top

[R76] 使用临时文件
来源：http://luf.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mmk.ydjk.org.cn

[R77] 读取用户输入
来源：http://gcf.xuanzx.com

read -rp "请输入: " ans
来源：http://jjz.ydzc1.top

[R78] 交互式菜单
来源：http://jzc.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ixb.gzhubu.top

[R79] 解析命令行选项
来源：http://xcj.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zxx.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://pzx.redwolf501.top

time ./run.sh
来源：http://paq.gaohongyu789.top

================================================================================
来源：http://taj.wangshuangyany.cn

S. C / C++ 专题
来源：http://nok.pengpengdd.cyou

================================================================================
来源：http://dzx.zhijiandao.cn

[S01] C：Hello World
来源：http://vxa.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://qxi.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://eit.guowangkeji.top

[S02] C：变量与格式化输出
来源：http://glb.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://duc.yuanzhike.top

[S03] C：读入整数
来源：http://sbu.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://rbo.aizwys.cn

[S04] C：字符串复制
来源：http://uva.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://juz.hfpthk.cn

[S05] C：字符串长度
来源：http://cav.svipenyu.cn

strlen(s)
来源：http://akr.guowangkeji.top

[S06] C：字符串比较
来源：http://zej.gzhubu.top

strcmp(a, b) == 0
来源：http://cav.guowangkeji.top

[S07] C：数组遍历求和
来源：http://kqn.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vwt.uphjek.com

[S08] C：动态内存分配与释放
来源：http://zyg.zdqjudy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hwa.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://wbt.fengsongda.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lxm.xylfe.cn

[S10] C：指针与解引用
来源：http://ohh.316326.xyz

int *p = &a;  *p = 5;
来源：http://yrh.cqqwz.cn

[S11] C：逐行读文件
来源：http://bgl.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://sms.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://odq.jyoumei.cn

fclose(f);
来源：http://ywo.gotoacloud.top

[S12] C：写文件
来源：http://hwy.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vzy.0kj1m.cn

[S13] C：宏定义
来源：http://rmz.yuxming.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zif.jqgfzy.top

[S14] C：枚举
来源：http://cpt.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://nnu.ybcxt.top

[S15] C：类型转换
来源：http://kuc.bbcook.cn

(double) a / b
来源：http://tzf.zdbjq.cn

[S16] C：位操作置位
来源：http://fon.gogol.net.cn

x |= (1 << 3);
来源：http://dbl.yongpay.top

[S17] C：安全拼接字符串
来源：http://pzu.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nhx.daxiang520.top

[S18] C：命令行参数
来源：http://fvy.quarkkingdee.top

int main(int argc, char **argv)
来源：http://hgz.tianlin.xyz

[S19] C：快速排序
来源：http://zel.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wil.gzhubu.top

[S20] C：二分查找
来源：http://zxo.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://agm.zhijiandao.cn

[S21] C：字符类别判断
来源：http://kkg.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yfa.redwolf501.top

[S22] C：字符串转数字
来源：http://zol.epnwcf.com

atoi("42");  strtod("3.14", NULL);
来源：http://wrj.yangfankeji.com

[S23] C：随机数
来源：http://yrd.fehbvm.com

srand(time(NULL));  int r = rand() % 100;
来源：http://jzj.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://cvn.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zek.ybcxt.top

[S25] C：内存拷贝
来源：http://yxs.yueranfly.top

memcpy(dst, src, n);
来源：http://hxz.tian-w.cn

[S26] C：内存清零
来源：http://qxw.316326.xyz

memset(a, 0, sizeof a);
来源：http://ygp.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://ozj.mhx1999.top

const double PI = 3.14159;
来源：http://chb.zhixingplan.top

[S28] C：静态变量
来源：http://wan.fzhhl.top

static int counter = 0;
来源：http://lny.nanxinkj.top

[S29] C：变参函数
来源：http://bhx.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://elg.nwbrower.top

[S30] C：头文件保护
来源：http://cna.vqdsnc.cn

#ifndef X_H
来源：http://ktw.0kj1m.cn

#define X_H
来源：http://tbm.dianchejie.cn

#endif
来源：http://mnc.dashuyun.cn

[S31] C++：Hello World
来源：http://fha.feifeiyinyue.top

#include <iostream>
来源：http://olt.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://vdb.smart0.xyz

[S32] C++：字符串
来源：http://gxm.daria6918.cn

std::string s = "hi";  s += "!";
来源：http://pkm.gogol.net.cn

[S33] C++：vector 增删
来源：http://bnw.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uaj.sysykeji.top

[S34] C++：遍历 vector
来源：http://ouc.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://uyv.yj20258888.top

[S35] C++：map
来源：http://qzx.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ixv.ivvv.top

[S36] C++：unordered_map
来源：http://lwx.nanxuanxn.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mwe.aizwys.cn

[S37] C++：set
来源：http://kcm.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pxm.ywan-chungtsiang.top

[S38] C++：排序
来源：http://qme.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://nbd.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://acn.aibaodan.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vel.shuidangran.top

[S40] C++：查找元素
来源：http://ylf.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ray.redwolf501.top

[S41] C++：类与构造函数
来源：http://bmb.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://moi.hnqzz.top

[S42] C++：继承与虚函数
来源：http://kph.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://ewb.zycfv.cn

[S43] C++：智能指针
来源：http://rzb.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://vvt.haohaochexian.top

[S44] C++：引用传参
来源：http://iyl.gzhubu.top

void inc(int &x) { ++x; }
来源：http://iil.fanxiaobao.xyz

[S45] C++：lambda
来源：http://hfw.gaohongyu789.top

auto add = [](int a, int b) { return a + b; };
来源：http://mhd.yj20258.top

[S46] C++：函数模板
来源：http://oje.jinqigufen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pew.52xcode.cn


<!-- 参考信息 -->