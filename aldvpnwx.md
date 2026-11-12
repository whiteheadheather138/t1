代发 wailian999

[Q76] 按天统计
来源：http://ybr.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kmd.jyoumei.cn

[Q77] 时间加减
来源：http://pfu.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://imv.hcnkem.com

[Q78] 当前时间
来源：http://nad.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://syn.tarul.cn

[Q79] 字符串拼接
来源：http://rxu.zycfv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://unm.daria6918.cn

[Q80] 字符串截取
来源：http://wxd.zhaomingkeji.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://noj.dianchejie.cn

[Q81] 字符串替换
来源：http://uks.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qhc.ivvv.top

[Q82] 字符长度与字节长度
来源：http://yys.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mkf.tarul.cn

[Q83] 大小写转换
来源：http://wif.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lzj.fengsongda.top

[Q84] 去除首尾空格
来源：http://ouy.haohaochexian.top

SELECT TRIM(name) FROM users;
来源：http://aya.zhixingplan.top

[Q85] 数值取整
来源：http://ziy.daria6918.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lar.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://kxp.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jgh.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://zcl.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://enn.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://jlu.nanxinkj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zad.quarkkingdee.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dad.birdmap.top

[Q89] 判断表是否存在
来源：http://nsf.sjlbkw.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cic.chenjidiqi.icu

[Q90] 生成序号列
来源：http://fwn.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pje.snrcjt.cn

================================================================================
来源：http://azh.yj20258888.top

R. Bash 专题
来源：http://zys.hongshengwenyu.top

================================================================================
来源：http://lqo.dashuyun.cn

[R01] shebang 与严格模式
来源：http://pap.kuanghao11.cn

#!/usr/bin/env bash
来源：http://shc.daria6918.cn

set -euo pipefail
来源：http://oql.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://kvz.epnwcf.com

name="Tom"; echo "$name"
来源：http://zzu.nanxinkj.top

[R03] 只读变量
来源：http://jzs.guowangkeji.top

readonly PI=3.14
来源：http://vhp.ydjk.org.cn

[R04] 位置参数
来源：http://vxg.vqdsnc.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bhc.hnqzz.top

[R05] 参数默认值
来源：http://jug.zhijiandao.cn

name="${1:-default}"
来源：http://bxo.52xcode.cn

[R06] 判断命令是否存在
来源：http://ybb.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ysw.smart0.xyz

[R07] if 判断文件
来源：http://fxk.andypj.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bpu.cashguo.top

[R08] 数值比较
来源：http://knk.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sth.jyoumei.cn

[R09] 字符串比较
来源：http://ipn.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qqp.birdmap.top

[R10] 正则匹配
来源：http://gwx.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zwm.sjlbkw.cn

[R11] case 多分支
来源：http://zie.ivvv.top

case "$1" in
来源：http://qhu.zhiwuduotai.top

start) echo "启动" ;;
来源：http://izn.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://ywb.hesvh.cn

*)     echo "未知命令" ;;
来源：http://fxd.sweek.top

esac
来源：http://zdm.zhixingplan.top

[R12] for 遍历文件
来源：http://hlg.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://sij.smart0.xyz

[R13] for 计数循环
来源：http://eac.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://zhw.xingfuxueyuan.xyz

[R14] C 风格 for
来源：http://qxj.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bvn.xziqi.cn

[R15] while 逐行读文件
来源：http://yjb.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wxv.gzhubu.top

[R16] until 等待条件
来源：http://ldq.ydjk.org.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ccb.aibaodan.cn

[R17] 数组定义与取值
来源：http://zas.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ivz.tian-w.cn

[R18] 遍历数组
来源：http://uvv.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://imu.cucudq.cn

[R19] 数组长度
来源：http://frz.ehwqpu.com

echo "${#arr[@]}"
来源：http://val.yongpay.top

[R20] 关联数组（字典）
来源：http://reg.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pbs.yj202588.top

[R21] 字符串长度
来源：http://jwq.wangshuangyany.cn

echo "${#s}"
来源：http://vkl.yonumen.top

[R22] 截取子串
来源：http://edr.chenjidiqi.icu

echo "${s:0:5}"
来源：http://tay.yonumen.top

[R23] 字符串替换
来源：http://bmm.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vks.ehwqpu.com

[R24] 大小写转换
来源：http://okh.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://maz.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://iwk.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kmi.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://mxr.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://ety.wangshuangyany.cn

[R27] 算术展开
来源：http://oqh.zhijiandao.cn

echo $((1 + 2 * 3))
来源：http://qht.sweek.top

[R28] 浮点运算
来源：http://gue.shanyushiyangtech.top

echo "scale=2; 10/3" | bc
来源：http://kzc.0kj1m.cn

[R29] 定义函数
来源：http://apl.quarkkingdee.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xoq.ctjpmb.com

[R30] 函数返回状态码
来源：http://adn.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://wiy.yj20258888.top

[R31] 局部变量
来源：http://lht.hesvh.cn

f() { local x=1; echo "$x"; }
来源：http://vwl.hnxiangtu.top

[R32] 参数个数校验
来源：http://gvx.tianlin.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ldw.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://biy.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ghr.aibaodan.cn

[R34] 退出时清理
来源：http://ohx.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zgi.snrcjt.cn

[R35] 后台执行并等待
来源：http://ipt.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://bwb.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://dzs.xylfe.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jbo.daxiang520.top

[R37] 把输出赋给变量
来源：http://azq.chenjidiqi.icu

files=$(ls -1)
来源：http://bek.yueranfly.top

[R38] 管道串联
来源：http://ugk.aizwys.cn

cat a.txt | grep -i error | wc -l
来源：http://qpj.pycfn.com

[R39] 重定向标准输出与错误
来源：http://gcf.ydzc1.top

cmd > out.log 2>&1
来源：http://trv.yuanzhike.top

[R40] 追加写日志
来源：http://bew.0kj1m.cn

echo "log" >> out.log
来源：http://yvi.aibaodan.cn

[R41] 丢弃输出
来源：http://ymn.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://fpu.yonumen.top

[R42] 输入重定向
来源：http://dyv.tian-w.cn

wc -l < a.txt
来源：http://gyv.shzxlz.cn

[R43] 按名字查找文件
来源：http://bxq.zhengqikj.top

find . -name "*.log" -type f
来源：http://sdc.jlsjyb.cn

[R44] 按修改时间查找
来源：http://vqm.yuxming.cn

find . -mtime -7 -type f
来源：http://mhi.hongshengwenyu.top

[R45] 批量删除
来源：http://umk.cucudq.cn

find . -name "*.tmp" -delete
来源：http://qco.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://wxy.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jin.tian-w.cn

[R47] sed 单行替换
来源：http://hnp.0kj1m.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wud.gzhubu.top

[R48] awk 取指定列
来源：http://tjo.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://azj.nanxinkj.top

[R49] awk 带条件
来源：http://cfg.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fgw.sysykeji.top

[R50] awk 求和
来源：http://pzh.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://ord.cucudq.cn

[R51] 排序去重取前几
来源：http://ejz.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://aeh.andypj.xyz

[R52] 统计行数
来源：http://bfw.ywan-chungtsiang.top

wc -l a.txt
来源：http://psy.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://pke.nanxinkj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ush.sysykeji.top

[R54] 比较两个文件
来源：http://pmc.yongpay.top

diff a.txt b.txt
来源：http://vgz.yvedp.cn

[R55] 压缩与解压
来源：http://glt.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hoo.ydzc1.top

[R56] 远程拷贝
来源：http://zsc.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://vuz.gaohongyu789.top

[R57] 远程执行命令
来源：http://ulg.ydjk.org.cn

ssh user@host 'uptime'
来源：http://wqf.tanke756.top

[R58] 下载文件
来源：http://coj.yvedp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://knb.xuanzx.com

[R59] 发 POST JSON
来源：http://kte.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iti.daria6918.cn

[R60] 只看 HTTP 状态码
来源：http://apw.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qyk.yonumen.top

[R61] 磁盘占用
来源：http://wwq.tian-w.cn

df -h;  du -sh *
来源：http://quk.0kj1m.cn

[R62] 找最占空间的文件
来源：http://aia.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://cry.jianghu66.top

[R63] 内存与进程
来源：http://hhu.dashuyun.cn

free -h;  ps aux | grep nginx
来源：http://xib.jiagoushi.top

[R64] 结束进程
来源：http://yyc.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://dyx.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://aqx.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ekn.ywan-chungtsiang.top

[R66] 定时任务
来源：http://lrn.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://xyn.yueranfly.top

[R67] 生成随机十六进制串
来源：http://dnv.jlsjyb.cn

openssl rand -hex 16
来源：http://wbq.gotoacloud.top

[R68] 计算文件校验值
来源：http://chw.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://nxp.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://rit.xylfe.cn

head -c 16 /dev/urandom | base64
来源：http://qla.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://znr.wangdashe.top

date +%s;  date -d @1700000000
来源：http://fsa.zdqjudy.top

[R71] 日期格式化
来源：http://hot.yongpay.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kfy.meibo888.top

[R72] 等待端口就绪
来源：http://lmt.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ode.cucudq.cn

[R73] 分割大日志
来源：http://bad.zycfv.cn

split -l 1000 big.log part_
来源：http://pkq.tianlin.xyz

[R74] 批量重命名
来源：http://lqv.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://znj.hysaishi.cn

[R75] 导出环境变量
来源：http://thn.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://css.yuanzhike.top

[R76] 使用临时文件
来源：http://lpi.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ibd.quarkkingdee.top

[R77] 读取用户输入
来源：http://nrl.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://lzj.yanxiufei.cn

[R78] 交互式菜单
来源：http://kyl.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://asg.sufxvd.cn

[R79] 解析命令行选项
来源：http://qbq.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ogg.snrcjt.cn

[R80] 查看脚本执行耗时
来源：http://yoy.gotoacloud.top

time ./run.sh
来源：http://fgq.tanke756.top

================================================================================
来源：http://clm.9152youxi.cn

S. C / C++ 专题
来源：http://gjt.yanxiufei.cn

================================================================================
来源：http://lzp.jyoumei.cn

[S01] C：Hello World
来源：http://rux.ctjpmb.com

#include <stdio.h>
来源：http://dmg.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://blb.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://zop.316326.xyz

int a = 10; printf("%d\n", a);
来源：http://jwy.jlsjyb.cn

[S03] C：读入整数
来源：http://dxk.gzhubu.top

int x; scanf("%d", &x);
来源：http://fiq.xylfe.cn

[S04] C：字符串复制
来源：http://sxq.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://eei.fehbvm.com

[S05] C：字符串长度
来源：http://kpo.zhiwuduotai.top

strlen(s)
来源：http://bvi.xziqi.cn

[S06] C：字符串比较
来源：http://ecf.smart0.xyz

strcmp(a, b) == 0
来源：http://vhl.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://byc.ywan-chungtsiang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rld.cdnleiting.top

[S08] C：动态内存分配与释放
来源：http://mzo.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ahv.feifeiyinyue.top

[S09] C：结构体定义与初始化
来源：http://qeo.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dpg.xziqi.cn

[S10] C：指针与解引用
来源：http://cid.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://vdr.ydjk.org.cn

[S11] C：逐行读文件
来源：http://spf.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://rtt.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://dtt.yuanzhike.top

fclose(f);
来源：http://ezp.fktsv.cn

[S12] C：写文件
来源：http://pxn.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://swh.0kj1m.cn

[S13] C：宏定义
来源：http://twx.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ytt.hywenlv.cn

[S14] C：枚举
来源：http://zen.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://kcs.jianghu66.top

[S15] C：类型转换
来源：http://gqo.vqdsnc.cn

(double) a / b
来源：http://ljy.yj20258.top

[S16] C：位操作置位
来源：http://etf.jyoumei.cn

x |= (1 << 3);
来源：http://qwo.daxiang520.top

[S17] C：安全拼接字符串
来源：http://srp.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ifi.daxiang520.top

[S18] C：命令行参数
来源：http://lfi.tanke756.top

int main(int argc, char **argv)
来源：http://lhe.ctjpmb.com

[S19] C：快速排序
来源：http://rqe.yongpay.top

qsort(a, n, sizeof(int), cmp);
来源：http://igr.cqqwz.cn

[S20] C：二分查找
来源：http://mwe.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vbt.hesvh.cn

[S21] C：字符类别判断
来源：http://gin.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ohz.cdnleiting.top

[S22] C：字符串转数字
来源：http://tbg.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://isu.cheryme.top

[S23] C：随机数
来源：http://yiz.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ezz.hysaishi.cn

[S24] C：获取本地时间
来源：http://eqh.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ypn.zhongyouzk.top

[S25] C：内存拷贝
来源：http://pgp.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://kmw.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://iak.yj202588.top

memset(a, 0, sizeof a);
来源：http://fuq.hfpthk.cn

[S27] C：定义常量
来源：http://ute.hongshengwenyu.top

const double PI = 3.14159;
来源：http://upv.guannengcc.top

[S28] C：静态变量
来源：http://bih.xylfe.cn

static int counter = 0;
来源：http://anq.smart0.xyz

[S29] C：变参函数
来源：http://dhk.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gyt.yfazqb.com

[S30] C：头文件保护
来源：http://vsp.0kj1m.cn

#ifndef X_H
来源：http://nkl.gzhubu.top

#define X_H
来源：http://kzm.ehwqpu.com

#endif
来源：http://srx.epnwcf.com

[S31] C++：Hello World
来源：http://pmh.yuxming.cn

#include <iostream>
来源：http://bzu.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://qcg.shanyushiyangtech.top

[S32] C++：字符串
来源：http://ojo.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://det.yonumen.top

[S33] C++：vector 增删
来源：http://inv.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vrw.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://ayy.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://xev.fktsv.cn

[S35] C++：map
来源：http://zxk.guowangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cwe.ctjpmb.com

[S36] C++：unordered_map
来源：http://lyw.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://foq.yj20258.top

[S37] C++：set
来源：http://tpv.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rap.yueranfly.top

[S38] C++：排序
来源：http://cnh.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://gxl.zycfv.cn

[S39] C++：自定义比较器排序
来源：http://yzo.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bbp.yongpay.top

[S40] C++：查找元素
来源：http://gdq.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dws.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://dcd.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rni.hammf.cn

[S42] C++：继承与虚函数
来源：http://wna.andypj.xyz

class B : public Base { public: void f() override {} };
来源：http://neq.zhoulong.xyz

[S43] C++：智能指针
来源：http://jso.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://irf.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://zfb.hesvh.cn

void inc(int &x) { ++x; }
来源：http://jfh.cheryme.top

[S45] C++：lambda
来源：http://thx.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://vzh.yj202588.top

[S46] C++：函数模板
来源：http://jmz.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qgo.hammf.cn


<!-- 参考信息 -->