代发 wailian999

[Q61] 移动平均
来源：http://cpy.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mpz.cheryme.top

[Q62] 分组占比
来源：http://btc.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zsw.tianlin.xyz

[Q63] 开启事务
来源：http://zpx.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sac.guannengcc.top

[Q64] 提交事务
来源：http://out.yj20258.top

COMMIT;
来源：http://evc.chenjidiqi.icu

[Q65] 回滚事务
来源：http://lih.cucudq.cn

ROLLBACK;
来源：http://fgn.fzhhl.top

[Q66] 行锁查询
来源：http://wpn.aibaodan.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gae.jiagoushi.top

[Q67] 设置隔离级别
来源：http://tlz.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xqq.redwolf501.top

[Q68] 保存点
来源：http://jka.shuidangran.top

SAVEPOINT sp1;
来源：http://vwc.dianchejie.cn

ROLLBACK TO sp1;
来源：http://hpx.mhx1999.top

[Q69] 查看执行计划
来源：http://vtb.gogol.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mkp.ctjpmb.com

[Q70] 更新统计信息
来源：http://hen.yonumen.top

ANALYZE TABLE users;
来源：http://aar.sweek.top

[Q71] 查看建表语句
来源：http://wtm.ywan-chungtsiang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ndi.epnwcf.com

[Q72] 查看索引
来源：http://nrs.xingfuxueyuan.xyz

SHOW INDEX FROM users;
来源：http://klr.kuanghao11.cn

[Q73] 查看表状态
来源：http://edx.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://jpb.fengsongda.top

[Q74] 强制使用索引
来源：http://vqt.shanyushiyangtech.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://frl.jlsjyb.cn

[Q75] 日期格式化
来源：http://dzy.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cfx.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://saz.yangfankeji.com

[Q76] 按天统计
来源：http://zww.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qcz.zhengqikj.top

[Q77] 时间加减
来源：http://jlv.vqdsnc.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nip.xylfe.cn

[Q78] 当前时间
来源：http://lww.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lju.mhx1999.top

[Q79] 字符串拼接
来源：http://tvg.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fnx.ydzc1.top

[Q80] 字符串截取
来源：http://lwb.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zjp.aizwys.cn

[Q81] 字符串替换
来源：http://hdw.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lbr.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://sfz.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://spn.tanke756.top

[Q83] 大小写转换
来源：http://xzj.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zad.jinqigufen.top

[Q84] 去除首尾空格
来源：http://swe.hfpthk.cn

SELECT TRIM(name) FROM users;
来源：http://ztk.pengpengdd.cyou

[Q85] 数值取整
来源：http://wbm.zdqjudy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xup.xziqi.cn

[Q86] 读取 JSON 字段
来源：http://cgk.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wtq.hongshengwenyu.top

[Q87] JSON 字段做条件
来源：http://usj.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mcj.yuxming.cn

[Q88] 行转列（条件聚合）
来源：http://pyp.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gqh.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dod.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://dna.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bun.kuanghao11.cn

[Q90] 生成序号列
来源：http://xsg.shuidangran.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oyl.jqgfzy.top

================================================================================
来源：http://xhl.zhengqikj.top

R. Bash 专题
来源：http://yjt.smart0.xyz

================================================================================
来源：http://bnc.xziqi.cn

[R01] shebang 与严格模式
来源：http://xjo.nanxinkj.top

#!/usr/bin/env bash
来源：http://bvf.guannengcc.top

set -euo pipefail
来源：http://pos.zhengqikj.top

[R02] 变量赋值与使用
来源：http://nvz.tianlin.xyz

name="Tom"; echo "$name"
来源：http://rwg.shanyushiyangtech.top

[R03] 只读变量
来源：http://xap.yj20258888.top

readonly PI=3.14
来源：http://fko.yfazqb.com

[R04] 位置参数
来源：http://ucr.quarkkingdee.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://opc.zycfv.cn

[R05] 参数默认值
来源：http://mpg.0kj1m.cn

name="${1:-default}"
来源：http://mri.ehwqpu.com

[R06] 判断命令是否存在
来源：http://chn.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://frc.sufxvd.cn

[R07] if 判断文件
来源：http://iga.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xqu.guowangkeji.top

[R08] 数值比较
来源：http://ztm.fengsongda.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bit.sysykeji.top

[R09] 字符串比较
来源：http://mlr.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ebs.xinyue.icu

[R10] 正则匹配
来源：http://dkh.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cxv.cucudq.cn

[R11] case 多分支
来源：http://hdm.pengpengdd.cyou

case "$1" in
来源：http://qxs.fktsv.cn

start) echo "启动" ;;
来源：http://zpu.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://uiq.c1oappe.top

*)     echo "未知命令" ;;
来源：http://gwb.fehbvm.com

esac
来源：http://ybw.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://qui.chenzaomai.com

for f in *.txt; do echo "$f"; done
来源：http://cis.birdmap.top

[R13] for 计数循环
来源：http://gwi.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://uwb.nanxinkj.top

[R14] C 风格 for
来源：http://kri.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lcj.tanke756.top

[R15] while 逐行读文件
来源：http://imj.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hfa.zdbjq.cn

[R16] until 等待条件
来源：http://pmz.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uxv.guannengcc.top

[R17] 数组定义与取值
来源：http://lgc.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://nkn.dianchejie.cn

[R18] 遍历数组
来源：http://otk.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qzz.svipenyu.cn

[R19] 数组长度
来源：http://orj.svipenyu.cn

echo "${#arr[@]}"
来源：http://qvn.yfazqb.com

[R20] 关联数组（字典）
来源：http://npu.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kds.shanyushiyangtech.top

[R21] 字符串长度
来源：http://zww.fengsongda.top

echo "${#s}"
来源：http://bad.wangdashe.top

[R22] 截取子串
来源：http://fwm.jiagoushi.top

echo "${s:0:5}"
来源：http://cvb.yonumen.top

[R23] 字符串替换
来源：http://lts.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lbx.zhixingplan.top

[R24] 大小写转换
来源：http://jsd.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vje.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://xfc.sweek.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dgr.iojbl.cn

[R26] 命令替换
来源：http://xuz.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://eme.jqgfzy.top

[R27] 算术展开
来源：http://qvn.zdbjq.cn

echo $((1 + 2 * 3))
来源：http://oam.quarkkingdee.top

[R28] 浮点运算
来源：http://fgp.52xcode.cn

echo "scale=2; 10/3" | bc
来源：http://xlq.gotoacloud.top

[R29] 定义函数
来源：http://taf.havefunace.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zku.xuanzx.com

[R30] 函数返回状态码
来源：http://kqd.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://vsi.aizwys.cn

[R31] 局部变量
来源：http://pdj.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://vns.meibo888.top

[R32] 参数个数校验
来源：http://cpf.hesvh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jlq.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://crr.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ydm.sjlbkw.cn

[R34] 退出时清理
来源：http://roh.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://owx.xuanzx.com

[R35] 后台执行并等待
来源：http://hnz.wangdashe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bkr.ydzc1.top

[R36] 并发执行多个任务
来源：http://zlt.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bas.hfpthk.cn

[R37] 把输出赋给变量
来源：http://lrd.tianlin.xyz

files=$(ls -1)
来源：http://mwv.shanyushiyangkeji.top

[R38] 管道串联
来源：http://tsw.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://yhv.hammf.cn

[R39] 重定向标准输出与错误
来源：http://qdn.cqqwz.cn

cmd > out.log 2>&1
来源：http://wcs.snrcjt.cn

[R40] 追加写日志
来源：http://ycl.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://cfj.bjfxy.top

[R41] 丢弃输出
来源：http://tui.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://bqj.ppjwa.cn

[R42] 输入重定向
来源：http://ngf.chenzaomai.com

wc -l < a.txt
来源：http://pbp.ydjk.org.cn

[R43] 按名字查找文件
来源：http://ynp.zhoulong.xyz

find . -name "*.log" -type f
来源：http://fwh.zhiwuduotai.top

[R44] 按修改时间查找
来源：http://vjm.birdmap.top

find . -mtime -7 -type f
来源：http://ihg.jinyuanbaomall.cn

[R45] 批量删除
来源：http://bkd.xingfuxueyuan.xyz

find . -name "*.tmp" -delete
来源：http://xcv.yj202588.top

[R46] 递归替换文件内容
来源：http://jts.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iwn.sysykeji.top

[R47] sed 单行替换
来源：http://tmi.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://czy.xylfe.cn

[R48] awk 取指定列
来源：http://aqq.jinyuanbaomall.cn

awk '{print $1, $3}' a.txt
来源：http://jyg.xuetiantiany.cn

[R49] awk 带条件
来源：http://jtb.smart0.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ywd.hysaishi.cn

[R50] awk 求和
来源：http://rkl.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://ocn.9152youxi.cn

[R51] 排序去重取前几
来源：http://yjc.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://daa.shanyushiyangkeji.top

[R52] 统计行数
来源：http://dbi.daxiang520.top

wc -l a.txt
来源：http://zhz.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://jao.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fsa.jiagoushi.top

[R54] 比较两个文件
来源：http://lwf.zycfv.cn

diff a.txt b.txt
来源：http://wdu.feifeiyinyue.top

[R55] 压缩与解压
来源：http://flr.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pvg.shangyingyoupin.top

[R56] 远程拷贝
来源：http://hoo.vqdsnc.cn

scp file user@host:/path/
来源：http://uhq.aibaodan.cn

[R57] 远程执行命令
来源：http://khg.hysaishi.cn

ssh user@host 'uptime'
来源：http://zsx.ivvv.top

[R58] 下载文件
来源：http://kpu.ehwqpu.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qvo.gzhubu.top

[R59] 发 POST JSON
来源：http://zbp.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wim.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://cnm.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://apu.guowangkeji.top

[R61] 磁盘占用
来源：http://mnf.cqqwz.cn

df -h;  du -sh *
来源：http://suo.daxiang520.top

[R62] 找最占空间的文件
来源：http://jdd.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://jsl.shanyushiyangkeji.top

[R63] 内存与进程
来源：http://qrn.sweek.top

free -h;  ps aux | grep nginx
来源：http://bmg.iojbl.cn

[R64] 结束进程
来源：http://esd.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://ees.hnxiangtu.top

[R65] 查看端口占用
来源：http://bqa.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xpj.shanyushiyangtech.top

[R66] 定时任务
来源：http://ylu.gzhubu.top

crontab -e;  crontab -l
来源：http://zhe.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://mcw.shzxlz.cn

openssl rand -hex 16
来源：http://ptu.tian-w.cn

[R68] 计算文件校验值
来源：http://cyi.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yea.hfpthk.cn

[R69] 生成随机密码
来源：http://gve.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://uwp.zhengqikj.top

[R70] 时间戳与互转
来源：http://eaz.hcnkem.com

date +%s;  date -d @1700000000
来源：http://dqt.zhixingplan.top

[R71] 日期格式化
来源：http://wxv.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fiq.hywenlv.cn

[R72] 等待端口就绪
来源：http://gvn.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://shu.aibaodan.cn

[R73] 分割大日志
来源：http://eum.hammf.cn

split -l 1000 big.log part_
来源：http://kxs.hongshengwenyu.top

[R74] 批量重命名
来源：http://opz.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fup.tianlin.xyz

[R75] 导出环境变量
来源：http://bxm.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://aum.xziqi.cn

[R76] 使用临时文件
来源：http://ptu.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cgk.ydjk.org.cn

[R77] 读取用户输入
来源：http://qft.c1oappe.top

read -rp "请输入: " ans
来源：http://wgj.guannengcc.top

[R78] 交互式菜单
来源：http://kqa.hywenlv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nwu.316326.xyz

[R79] 解析命令行选项
来源：http://hip.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eci.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://exy.zdqjudy.top

time ./run.sh
来源：http://cdy.cashguo.top

================================================================================
来源：http://bky.yangfankeji.com

S. C / C++ 专题
来源：http://qdy.zhaomingkeji.xyz

================================================================================
来源：http://swo.yonumen.top

[S01] C：Hello World
来源：http://ydv.jqgufenzy.top

#include <stdio.h>
来源：http://ghx.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vzf.bbcook.cn

[S02] C：变量与格式化输出
来源：http://blx.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://drv.tianlin.xyz

[S03] C：读入整数
来源：http://fjw.bbcook.cn

int x; scanf("%d", &x);
来源：http://zfq.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://krk.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://ulm.wangdashe.top

[S05] C：字符串长度
来源：http://wzh.zhixingplan.top

strlen(s)
来源：http://bvv.iojbl.cn

[S06] C：字符串比较
来源：http://pps.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://cpi.jyoumei.cn

[S07] C：数组遍历求和
来源：http://rkb.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wpp.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://zkk.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ozr.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://tdn.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iuc.chenlongwang.top

[S10] C：指针与解引用
来源：http://nar.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://ucq.hcnkem.com

[S11] C：逐行读文件
来源：http://kvm.iojbl.cn

FILE *f = fopen("a.txt", "r");
来源：http://oht.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dit.zdbjq.cn

fclose(f);
来源：http://qmo.zhongyouzk.top

[S12] C：写文件
来源：http://nbr.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://krf.hywenlv.cn

[S13] C：宏定义
来源：http://cqr.ctjpmb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://saj.dashuyun.cn

[S14] C：枚举
来源：http://saa.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://agr.tanke756.top

[S15] C：类型转换
来源：http://mpx.bjfxy.top

(double) a / b
来源：http://osu.redwolf501.top

[S16] C：位操作置位
来源：http://jie.shanyushiyangtech.top

x |= (1 << 3);
来源：http://qpq.hcnkem.com

[S17] C：安全拼接字符串
来源：http://tfp.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oke.yj202588.top

[S18] C：命令行参数
来源：http://gwl.aizwys.cn

int main(int argc, char **argv)
来源：http://agx.ivvv.top

[S19] C：快速排序
来源：http://oqv.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xyp.mhx1999.top

[S20] C：二分查找
来源：http://djz.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hrh.guowangkeji.top

[S21] C：字符类别判断
来源：http://qbg.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://srb.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://xzb.hfpthk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://unf.sysykeji.top

[S23] C：随机数
来源：http://lkf.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://abr.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://yaf.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rjq.aibaodan.cn

[S25] C：内存拷贝
来源：http://wla.sysykeji.top

memcpy(dst, src, n);
来源：http://jdf.hnxiangtu.top

[S26] C：内存清零
来源：http://ruy.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://whq.yongpay.top

[S27] C：定义常量
来源：http://fcg.ydjk.org.cn

const double PI = 3.14159;
来源：http://yxl.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://omb.meibo888.top

static int counter = 0;
来源：http://loo.dianchejie.cn

[S29] C：变参函数
来源：http://dpo.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hds.yj20258.top

[S30] C：头文件保护
来源：http://lmk.ppjwa.cn

#ifndef X_H
来源：http://fys.jyoumei.cn

#define X_H
来源：http://mux.yj20258.top

#endif
来源：http://bgy.cashguo.top

[S31] C++：Hello World
来源：http://fzv.jinqigufen.top


<!-- 参考信息 -->