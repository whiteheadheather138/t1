代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eba.zycfv.cn

[Q75] 日期格式化
来源：http://xgy.nanxuanxn.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yei.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hfa.hongshengwenyu.top

[Q76] 按天统计
来源：http://gsc.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ovl.ybcxt.top

[Q77] 时间加减
来源：http://ejq.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tbs.hesvh.cn

[Q78] 当前时间
来源：http://dud.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ncb.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://env.zycfv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vxm.nwbrower.top

[Q80] 字符串截取
来源：http://bna.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dqa.yonumen.top

[Q81] 字符串替换
来源：http://fkf.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bav.hammf.cn

[Q82] 字符长度与字节长度
来源：http://ssf.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ocx.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://gte.ybcxt.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cyj.vehdjk.com

[Q84] 去除首尾空格
来源：http://ehx.yj20258.top

SELECT TRIM(name) FROM users;
来源：http://ray.hesvh.cn

[Q85] 数值取整
来源：http://dkr.epnwcf.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lve.yueranfly.top

[Q86] 读取 JSON 字段
来源：http://kxv.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ytv.yongpay.top

[Q87] JSON 字段做条件
来源：http://coi.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fzu.shanyushiyangkeji.top

[Q88] 行转列（条件聚合）
来源：http://onq.gaohongyu789.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hht.shuidangran.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ija.daxiang520.top

[Q89] 判断表是否存在
来源：http://haa.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vec.gzhubu.top

[Q90] 生成序号列
来源：http://ycg.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wcz.316326.xyz

================================================================================
来源：http://rcf.svipenyu.cn

R. Bash 专题
来源：http://xxy.xziqi.cn

================================================================================
来源：http://put.shuidangran.top

[R01] shebang 与严格模式
来源：http://zdt.mhx1999.top

#!/usr/bin/env bash
来源：http://yax.ybcxt.top

set -euo pipefail
来源：http://reb.guannengcc.top

[R02] 变量赋值与使用
来源：http://xet.feifeiyinyue.top

name="Tom"; echo "$name"
来源：http://yrz.aibaodan.cn

[R03] 只读变量
来源：http://lcq.9152youxi.cn

readonly PI=3.14
来源：http://uhp.haohaochexian.top

[R04] 位置参数
来源：http://qgd.jqgufenzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gum.aibaodan.cn

[R05] 参数默认值
来源：http://ugm.fzhhl.top

name="${1:-default}"
来源：http://jew.xuanzx.com

[R06] 判断命令是否存在
来源：http://hev.pengpengdd.cyou

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yef.svipenyu.cn

[R07] if 判断文件
来源：http://uge.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uxk.yj202588.top

[R08] 数值比较
来源：http://lwa.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://okp.shzxlz.cn

[R09] 字符串比较
来源：http://vxe.xingfuxueyuan.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ngs.0kj1m.cn

[R10] 正则匹配
来源：http://kns.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yvt.cucudq.cn

[R11] case 多分支
来源：http://ixr.sufxvd.cn

case "$1" in
来源：http://pvr.shangyingyoupin.top

start) echo "启动" ;;
来源：http://vnn.0kj1m.cn

stop)  echo "停止" ;;
来源：http://nev.nwbrower.top

*)     echo "未知命令" ;;
来源：http://xxn.havefunace.top

esac
来源：http://qda.fzhhl.top

[R12] for 遍历文件
来源：http://mrg.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://uvb.sweek.top

[R13] for 计数循环
来源：http://eve.zhixingplan.top

for i in {1..10}; do echo "$i"; done
来源：http://yzj.quarkkingdee.top

[R14] C 风格 for
来源：http://how.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cbc.jlsjyb.cn

[R15] while 逐行读文件
来源：http://lea.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fsd.fktsv.cn

[R16] until 等待条件
来源：http://rru.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mvd.fzhhl.top

[R17] 数组定义与取值
来源：http://jjv.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uwb.yj202588.top

[R18] 遍历数组
来源：http://nzf.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qyv.zdbjq.cn

[R19] 数组长度
来源：http://blq.sufxvd.cn

echo "${#arr[@]}"
来源：http://mad.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://zzv.ehwqpu.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gjr.yfazqb.com

[R21] 字符串长度
来源：http://rxz.jqgufenzy.top

echo "${#s}"
来源：http://ugy.zycfv.cn

[R22] 截取子串
来源：http://gho.shangyingyoupin.top

echo "${s:0:5}"
来源：http://wug.ivvv.top

[R23] 字符串替换
来源：http://meq.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mud.hongshengwenyu.top

[R24] 大小写转换
来源：http://uuv.hcnkem.com

echo "${s^^}"; echo "${s,,}"
来源：http://bxm.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://ahw.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vqo.xziqi.cn

[R26] 命令替换
来源：http://hdi.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://pwx.shanyushiyangtech.top

[R27] 算术展开
来源：http://oso.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://dct.dashuyun.cn

[R28] 浮点运算
来源：http://xar.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://rco.xylfe.cn

[R29] 定义函数
来源：http://aym.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://usf.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://bzi.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://quf.nanxinkj.top

[R31] 局部变量
来源：http://wrv.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://fow.nwbrower.top

[R32] 参数个数校验
来源：http://siv.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mpe.fktsv.cn

[R33] 捕获错误并提示行号
来源：http://tmg.kuanghao11.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ilr.gzhubu.top

[R34] 退出时清理
来源：http://ybf.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://yzz.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://nvx.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ynx.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://vej.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bkx.gzhubu.top

[R37] 把输出赋给变量
来源：http://mcf.316326.xyz

files=$(ls -1)
来源：http://ryz.9152youxi.cn

[R38] 管道串联
来源：http://ztj.yuanzhike.top

cat a.txt | grep -i error | wc -l
来源：http://zov.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://edg.ppjwa.cn

cmd > out.log 2>&1
来源：http://bpw.gogol.net.cn

[R40] 追加写日志
来源：http://tkk.daria6918.cn

echo "log" >> out.log
来源：http://mcz.yueranfly.top

[R41] 丢弃输出
来源：http://zgf.zhaomingkeji.xyz

cmd >/dev/null 2>&1
来源：http://jkx.sufxvd.cn

[R42] 输入重定向
来源：http://nvz.ctjpmb.com

wc -l < a.txt
来源：http://lyv.tanke756.top

[R43] 按名字查找文件
来源：http://ayd.sufxvd.cn

find . -name "*.log" -type f
来源：http://xaq.gzhubu.top

[R44] 按修改时间查找
来源：http://obt.gogol.net.cn

find . -mtime -7 -type f
来源：http://dqo.haohaochexian.top

[R45] 批量删除
来源：http://kmp.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://zlf.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://yii.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uix.jqgufenzy.top

[R47] sed 单行替换
来源：http://kzu.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://kjq.ywan-chungtsiang.top

[R48] awk 取指定列
来源：http://lsj.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://qkx.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://xmq.zhengqikj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://utd.jqgufenzy.top

[R50] awk 求和
来源：http://wzo.shangyingyoupin.top

awk '{s += $2} END {print s}' a.txt
来源：http://rnp.sjlbkw.cn

[R51] 排序去重取前几
来源：http://azq.gotoacloud.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gxt.guannengcc.top

[R52] 统计行数
来源：http://qap.feifeiyinyue.top

wc -l a.txt
来源：http://jnm.yuanzhike.top

[R53] 查看文件头与实时尾
来源：http://iix.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ddt.fengsongda.top

[R54] 比较两个文件
来源：http://idc.aibaodan.cn

diff a.txt b.txt
来源：http://foc.jqgfzy.top

[R55] 压缩与解压
来源：http://bhb.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jlv.xuanzx.com

[R56] 远程拷贝
来源：http://qps.dashuyun.cn

scp file user@host:/path/
来源：http://wri.xylfe.cn

[R57] 远程执行命令
来源：http://zku.gaohongyu789.top

ssh user@host 'uptime'
来源：http://axr.dianchejie.cn

[R58] 下载文件
来源：http://pka.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ets.jyoumei.cn

[R59] 发 POST JSON
来源：http://ajg.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nqu.kuanghao11.cn

[R60] 只看 HTTP 状态码
来源：http://vhs.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://azr.ppjwa.cn

[R61] 磁盘占用
来源：http://awl.xylfe.cn

df -h;  du -sh *
来源：http://hph.nanxinkj.top

[R62] 找最占空间的文件
来源：http://icl.shuidangran.top

du -ah . | sort -rh | head -10
来源：http://uxf.xinyue.icu

[R63] 内存与进程
来源：http://igq.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://krv.tanke756.top

[R64] 结束进程
来源：http://bej.feifeiyinyue.top

kill -9 $(pgrep -f app.py)
来源：http://hhu.dashuyun.cn

[R65] 查看端口占用
来源：http://pww.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xep.feifeiyinyue.top

[R66] 定时任务
来源：http://lbq.zhixingplan.top

crontab -e;  crontab -l
来源：http://nfu.zhiwuduotai.top

[R67] 生成随机十六进制串
来源：http://ndc.xuanzx.com

openssl rand -hex 16
来源：http://ibb.hywenlv.cn

[R68] 计算文件校验值
来源：http://bnm.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://ako.ydjk.org.cn

[R69] 生成随机密码
来源：http://wpk.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://dbo.daxiang520.top

[R70] 时间戳与互转
来源：http://xnq.cashguo.top

date +%s;  date -d @1700000000
来源：http://lqj.gzhubu.top

[R71] 日期格式化
来源：http://zuv.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bso.birdmap.top

[R72] 等待端口就绪
来源：http://bhx.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://isb.yonumen.top

[R73] 分割大日志
来源：http://otv.jqgufenzy.top

split -l 1000 big.log part_
来源：http://obn.xinyue.icu

[R74] 批量重命名
来源：http://aok.xuetiantiany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zcp.ydzc1.top

[R75] 导出环境变量
来源：http://hqt.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://rsn.nanxuanxn.top

[R76] 使用临时文件
来源：http://lrx.ehwqpu.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gal.dianchejie.cn

[R77] 读取用户输入
来源：http://kgm.zhijiandao.cn

read -rp "请输入: " ans
来源：http://fms.zhiwuduotai.top

[R78] 交互式菜单
来源：http://sew.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hzs.sjlbkw.cn

[R79] 解析命令行选项
来源：http://fps.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jjq.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://wgt.chenzaomai.com

time ./run.sh
来源：http://zrd.yj20258.top

================================================================================
来源：http://cqy.shanyushiyangkeji.top

S. C / C++ 专题
来源：http://nbw.nanxuanxn.top

================================================================================
来源：http://yco.jyoumei.cn

[S01] C：Hello World
来源：http://zuj.guowangkeji.top

#include <stdio.h>
来源：http://uiz.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://prm.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://haw.zhaomingkeji.xyz

int a = 10; printf("%d\n", a);
来源：http://uap.bjfxy.top

[S03] C：读入整数
来源：http://jxd.yangfankeji.com

int x; scanf("%d", &x);
来源：http://lrs.andypj.xyz

[S04] C：字符串复制
来源：http://tje.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://lxc.ppjwa.cn

[S05] C：字符串长度
来源：http://yea.aizwys.cn

strlen(s)
来源：http://kvu.gzhubu.top

[S06] C：字符串比较
来源：http://iqg.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://mlx.sufxvd.cn

[S07] C：数组遍历求和
来源：http://kib.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kzq.jiagoushi.top

[S08] C：动态内存分配与释放
来源：http://aai.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zzi.jinqigufen.top

[S09] C：结构体定义与初始化
来源：http://bvi.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kaj.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://lki.jianghu66.top

int *p = &a;  *p = 5;
来源：http://kii.sxryk.cn

[S11] C：逐行读文件
来源：http://ilu.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://cyv.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fwl.jlsjyb.cn

fclose(f);
来源：http://auf.chenjidiqi.icu

[S12] C：写文件
来源：http://pxv.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hgk.yj202588.top

[S13] C：宏定义
来源：http://hyl.jinghuilouyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qkw.shzxlz.cn

[S14] C：枚举
来源：http://jdv.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://ebh.jqgfzy.top

[S15] C：类型转换
来源：http://lho.pengpengdd.cyou

(double) a / b
来源：http://kdy.smart0.xyz

[S16] C：位操作置位
来源：http://krf.yonumen.top

x |= (1 << 3);
来源：http://cms.yonumen.top

[S17] C：安全拼接字符串
来源：http://fmh.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zlj.redwolf501.top

[S18] C：命令行参数
来源：http://mkw.yfazqb.com

int main(int argc, char **argv)
来源：http://ouk.jlsjyb.cn

[S19] C：快速排序
来源：http://iry.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://czb.chenzaomai.com

[S20] C：二分查找
来源：http://bys.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rlr.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://aqo.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eqk.9152youxi.cn

[S22] C：字符串转数字
来源：http://zui.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://awt.zhiwuduotai.top

[S23] C：随机数
来源：http://neb.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dgq.shuidangran.top

[S24] C：获取本地时间
来源：http://kpk.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://siz.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://dba.chenzaomai.com

memcpy(dst, src, n);
来源：http://fkg.316326.xyz

[S26] C：内存清零
来源：http://mpe.bjfxy.top

memset(a, 0, sizeof a);
来源：http://ohr.dashuyun.cn

[S27] C：定义常量
来源：http://bql.yj20258888.top

const double PI = 3.14159;
来源：http://hyo.wangshuangyany.cn

[S28] C：静态变量
来源：http://bzl.xziqi.cn

static int counter = 0;
来源：http://glf.fanxiaobao.xyz

[S29] C：变参函数
来源：http://qoj.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vyr.ydzc1.top

[S30] C：头文件保护
来源：http://maz.shzxlz.cn

#ifndef X_H
来源：http://ouo.xuetiantiany.cn

#define X_H
来源：http://oup.ybcxt.top

#endif
来源：http://qmd.nanxuanxn.top

[S31] C++：Hello World
来源：http://tmy.tanke756.top

#include <iostream>
来源：http://cwb.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ovk.52xcode.cn

[S32] C++：字符串
来源：http://qwm.uphjek.com

std::string s = "hi";  s += "!";
来源：http://ork.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://ybz.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kmq.aizwys.cn

[S34] C++：遍历 vector
来源：http://rzg.52xcode.cn

for (auto &x : v) { std::cout << x; }
来源：http://sgx.nanxuanxn.top

[S35] C++：map
来源：http://jdr.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mfl.ivvv.top

[S36] C++：unordered_map
来源：http://omf.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lzi.iojbl.cn

[S37] C++：set
来源：http://wjh.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xhy.jlsjyb.cn

[S38] C++：排序
来源：http://iqc.ehwqpu.com

std::sort(v.begin(), v.end());
来源：http://nmy.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://csp.gzhubu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vqs.jinghuilouyu.cn

[S40] C++：查找元素
来源：http://rpz.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://edh.shanyushiyangtech.top

[S41] C++：类与构造函数
来源：http://uja.gzhubu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nvy.jinqigufen.top

[S42] C++：继承与虚函数
来源：http://xpb.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://wfw.ydjk.org.cn

[S43] C++：智能指针
来源：http://txa.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://dxj.sjlbkw.cn

[S44] C++：引用传参
来源：http://asf.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://sgr.jqgufenzy.top


<!-- 参考信息 -->