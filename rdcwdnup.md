代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vvk.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://mis.sjlbkw.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mvv.hnqzz.top

[Q57] 行号
来源：http://kqz.sjlbkw.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lcl.yanxiufei.cn

[Q58] 累计求和
来源：http://njm.dashuyun.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ybc.zdqjudy.top

[Q59] 分组内累计
来源：http://xfl.daria6918.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fmw.hammf.cn

[Q60] 取上一行 / 下一行
来源：http://wqg.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rgk.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://arg.shangyingyoupin.top

[Q61] 移动平均
来源：http://pjg.redwolf501.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wza.316326.xyz

[Q62] 分组占比
来源：http://rzt.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xmp.wangdashe.top

[Q63] 开启事务
来源：http://aeg.wangshuangyany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://axn.chenlongwang.top

[Q64] 提交事务
来源：http://lzf.dianchejie.cn

COMMIT;
来源：http://xad.zhixingplan.top

[Q65] 回滚事务
来源：http://nfx.daria6918.cn

ROLLBACK;
来源：http://dvj.dianchejie.cn

[Q66] 行锁查询
来源：http://amz.tianlin.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bip.316326.xyz

[Q67] 设置隔离级别
来源：http://ceq.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jnt.gaohongyu789.top

[Q68] 保存点
来源：http://svq.daria6918.cn

SAVEPOINT sp1;
来源：http://grl.c1oappe.top

ROLLBACK TO sp1;
来源：http://ilr.yj20258.top

[Q69] 查看执行计划
来源：http://xum.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://svl.52xcode.cn

[Q70] 更新统计信息
来源：http://swd.snrcjt.cn

ANALYZE TABLE users;
来源：http://cxg.dashuyun.cn

[Q71] 查看建表语句
来源：http://zze.aibaodan.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://buj.jinqigufen.top

[Q72] 查看索引
来源：http://trv.iojbl.cn

SHOW INDEX FROM users;
来源：http://lhj.tianlin.xyz

[Q73] 查看表状态
来源：http://zxj.52xcode.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uhq.yanxiufei.cn

[Q74] 强制使用索引
来源：http://jpv.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fyu.hongshengwenyu.top

[Q75] 日期格式化
来源：http://ddv.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dia.hammf.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zgt.iojbl.cn

[Q76] 按天统计
来源：http://jcw.shanyushiyangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dfq.nwbrower.top

[Q77] 时间加减
来源：http://irn.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bpq.feifeiyinyue.top

[Q78] 当前时间
来源：http://enk.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kmf.jqgufenzy.top

[Q79] 字符串拼接
来源：http://bil.pycfn.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qxe.andypj.xyz

[Q80] 字符串截取
来源：http://dmp.bbcook.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iqs.zdbjq.cn

[Q81] 字符串替换
来源：http://dun.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sfi.xingfuxueyuan.xyz

[Q82] 字符长度与字节长度
来源：http://ufz.tianlin.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qfh.redwolf501.top

[Q83] 大小写转换
来源：http://beu.zhengqikj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cgm.52xcode.cn

[Q84] 去除首尾空格
来源：http://uhn.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://oyp.jqgfzy.top

[Q85] 数值取整
来源：http://brx.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uwm.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://doq.shzxlz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://emh.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://hsk.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://icg.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://cys.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ddo.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iof.sxryk.cn

[Q89] 判断表是否存在
来源：http://ibe.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nts.hcnkem.com

[Q90] 生成序号列
来源：http://gpp.andypj.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rto.hywenlv.cn

================================================================================
来源：http://mwg.xziqi.cn

R. Bash 专题
来源：http://bsg.yuxming.cn

================================================================================
来源：http://rvn.hywenlv.cn

[R01] shebang 与严格模式
来源：http://wts.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://yqn.tianlin.xyz

set -euo pipefail
来源：http://wpp.gotoacloud.top

[R02] 变量赋值与使用
来源：http://xru.cucudq.cn

name="Tom"; echo "$name"
来源：http://rbj.yuxming.cn

[R03] 只读变量
来源：http://ivi.zhijiandao.cn

readonly PI=3.14
来源：http://vtm.zhijiandao.cn

[R04] 位置参数
来源：http://puq.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mua.hongshengwenyu.top

[R05] 参数默认值
来源：http://csb.nanxinkj.top

name="${1:-default}"
来源：http://ibe.hysaishi.cn

[R06] 判断命令是否存在
来源：http://kmq.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cjv.fktsv.cn

[R07] if 判断文件
来源：http://llq.tian-w.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pjq.wangshuangyany.cn

[R08] 数值比较
来源：http://wue.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uus.jinyuanbaomall.cn

[R09] 字符串比较
来源：http://fqt.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jez.dashuyun.cn

[R10] 正则匹配
来源：http://rej.gzhubu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jlr.quarkkingdee.top

[R11] case 多分支
来源：http://xum.fanxiaobao.xyz

case "$1" in
来源：http://fkp.zdqjudy.top

start) echo "启动" ;;
来源：http://tpq.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://maz.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://xgu.zhijiandao.cn

esac
来源：http://zqz.ydzc1.top

[R12] for 遍历文件
来源：http://ihd.bbcook.cn

for f in *.txt; do echo "$f"; done
来源：http://gdg.jinghuilouyu.cn

[R13] for 计数循环
来源：http://ubw.ywan-chungtsiang.top

for i in {1..10}; do echo "$i"; done
来源：http://omc.tianlin.xyz

[R14] C 风格 for
来源：http://rjt.smart0.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xlp.cdnleiting.top

[R15] while 逐行读文件
来源：http://dby.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://omo.yongpay.top

[R16] until 等待条件
来源：http://jwf.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gej.fehbvm.com

[R17] 数组定义与取值
来源：http://xhf.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://qcg.sweek.top

[R18] 遍历数组
来源：http://ive.jyoumei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gxw.zhaomingkeji.xyz

[R19] 数组长度
来源：http://exb.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://bay.redwolf501.top

[R20] 关联数组（字典）
来源：http://ifa.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dlz.hysaishi.cn

[R21] 字符串长度
来源：http://fal.quarkkingdee.top

echo "${#s}"
来源：http://kty.jqgufenzy.top

[R22] 截取子串
来源：http://vjo.gzhubu.top

echo "${s:0:5}"
来源：http://eto.jinqigfzy.top

[R23] 字符串替换
来源：http://cvp.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://log.chenlongwang.top

[R24] 大小写转换
来源：http://xoe.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qsq.gogol.net.cn

[R25] 去后缀 / 去前缀
来源：http://pon.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lwv.aizwys.cn

[R26] 命令替换
来源：http://orh.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://ewb.daxiang520.top

[R27] 算术展开
来源：http://roj.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://jsl.gzhubu.top

[R28] 浮点运算
来源：http://rbm.chenzaomai.com

echo "scale=2; 10/3" | bc
来源：http://fwr.gogol.net.cn

[R29] 定义函数
来源：http://dco.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qzy.yvedp.cn

[R30] 函数返回状态码
来源：http://ssg.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://mtq.fanxiaobao.xyz

[R31] 局部变量
来源：http://fpz.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://qhs.wangshuangyany.cn

[R32] 参数个数校验
来源：http://huh.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vkc.ywan-chungtsiang.top

[R33] 捕获错误并提示行号
来源：http://lvp.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vgx.ivvv.top

[R34] 退出时清理
来源：http://lrx.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://qcr.jinqigufen.top

[R35] 后台执行并等待
来源：http://dwt.chenjidiqi.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://rom.cucudq.cn

[R36] 并发执行多个任务
来源：http://tra.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://thb.zdqjudy.top

[R37] 把输出赋给变量
来源：http://ews.yvedp.cn

files=$(ls -1)
来源：http://ncg.zhoulong.xyz

[R38] 管道串联
来源：http://jki.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://moz.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://gpm.andypj.xyz

cmd > out.log 2>&1
来源：http://bch.dianchejie.cn

[R40] 追加写日志
来源：http://ywk.tanke756.top

echo "log" >> out.log
来源：http://cye.316326.xyz

[R41] 丢弃输出
来源：http://zmm.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://uwl.nanxuanxn.top

[R42] 输入重定向
来源：http://axt.kuanghao11.cn

wc -l < a.txt
来源：http://syr.0kj1m.cn

[R43] 按名字查找文件
来源：http://igg.9152youxi.cn

find . -name "*.log" -type f
来源：http://qiy.bbcook.cn

[R44] 按修改时间查找
来源：http://tbz.hfpthk.cn

find . -mtime -7 -type f
来源：http://mmd.chenjidiqi.icu

[R45] 批量删除
来源：http://loe.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://bzb.gzhubu.top

[R46] 递归替换文件内容
来源：http://iiw.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hyl.hongshengwenyu.top

[R47] sed 单行替换
来源：http://zka.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://vyn.haohaochexian.top

[R48] awk 取指定列
来源：http://rvp.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://xzw.0kj1m.cn

[R49] awk 带条件
来源：http://oet.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bjb.jinqigfzy.top

[R50] awk 求和
来源：http://bgg.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://jbr.xylfe.cn

[R51] 排序去重取前几
来源：http://pdv.feifeiyinyue.top

sort a.txt | uniq -c | sort -rn | head
来源：http://eih.xinyue.icu

[R52] 统计行数
来源：http://ppi.sufxvd.cn

wc -l a.txt
来源：http://ejq.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://nsq.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qwb.hammf.cn

[R54] 比较两个文件
来源：http://hod.gaohongyu789.top

diff a.txt b.txt
来源：http://bpe.svipenyu.cn

[R55] 压缩与解压
来源：http://ywl.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fpn.jianghu66.top

[R56] 远程拷贝
来源：http://kxq.aizwys.cn

scp file user@host:/path/
来源：http://uje.aibaodan.cn

[R57] 远程执行命令
来源：http://tmp.zhixingplan.top

ssh user@host 'uptime'
来源：http://keg.cheryme.top

[R58] 下载文件
来源：http://ipn.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ixp.jqgufenzy.top

[R59] 发 POST JSON
来源：http://rse.hysaishi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kth.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://tyl.wangdashe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://evr.hesvh.cn

[R61] 磁盘占用
来源：http://vvh.pycfn.com

df -h;  du -sh *
来源：http://fsb.fehbvm.com

[R62] 找最占空间的文件
来源：http://lug.shuidangran.top

du -ah . | sort -rh | head -10
来源：http://gmu.yanxiufei.cn

[R63] 内存与进程
来源：http://svd.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://myn.hfpthk.cn

[R64] 结束进程
来源：http://xdc.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://uxj.fzhhl.top

[R65] 查看端口占用
来源：http://ihe.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yxa.daxiang520.top

[R66] 定时任务
来源：http://kqs.yangfankeji.com

crontab -e;  crontab -l
来源：http://oqz.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://mhv.hammf.cn

openssl rand -hex 16
来源：http://nnw.hnqzz.top

[R68] 计算文件校验值
来源：http://yjl.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://deb.zycfv.cn

[R69] 生成随机密码
来源：http://mqf.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://vyj.sufxvd.cn

[R70] 时间戳与互转
来源：http://fds.ydzc1.top

date +%s;  date -d @1700000000
来源：http://pyk.havefunace.top

[R71] 日期格式化
来源：http://fcj.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hyp.hfpthk.cn

[R72] 等待端口就绪
来源：http://ccg.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rtx.yj20258888.top

[R73] 分割大日志
来源：http://moo.yfazqb.com

split -l 1000 big.log part_
来源：http://vxu.jinqigfzy.top

[R74] 批量重命名
来源：http://cth.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://scc.jlsjyb.cn

[R75] 导出环境变量
来源：http://cxv.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://idi.jinyuanbaomall.cn

[R76] 使用临时文件
来源：http://ass.jyoumei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vwc.fengsongda.top

[R77] 读取用户输入
来源：http://uld.ydjk.org.cn

read -rp "请输入: " ans
来源：http://lvm.zdbjq.cn

[R78] 交互式菜单
来源：http://fcf.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qqi.aizwys.cn

[R79] 解析命令行选项
来源：http://aby.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://txh.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://cfo.guannengcc.top

time ./run.sh
来源：http://orn.yonumen.top

================================================================================
来源：http://dqy.sufxvd.cn

S. C / C++ 专题
来源：http://wzj.yonumen.top

================================================================================
来源：http://lky.fengsongda.top

[S01] C：Hello World
来源：http://qdp.svipenyu.cn

#include <stdio.h>
来源：http://hbt.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://clb.birdmap.top

[S02] C：变量与格式化输出
来源：http://nbq.zhoulong.xyz

int a = 10; printf("%d\n", a);
来源：http://xlu.jianghu66.top

[S03] C：读入整数
来源：http://qyw.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://tam.yuxming.cn

[S04] C：字符串复制
来源：http://idq.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xbh.guowangkeji.top

[S05] C：字符串长度
来源：http://vet.yfazqb.com

strlen(s)
来源：http://png.zhengqikj.top

[S06] C：字符串比较
来源：http://ctf.yuanzhike.top

strcmp(a, b) == 0
来源：http://ced.ywan-chungtsiang.top

[S07] C：数组遍历求和
来源：http://vxd.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dyn.jyoumei.cn

[S08] C：动态内存分配与释放
来源：http://jps.aizwys.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bcf.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://led.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jdi.andypj.xyz

[S10] C：指针与解引用
来源：http://rmx.xylfe.cn

int *p = &a;  *p = 5;
来源：http://pfz.gogol.net.cn

[S11] C：逐行读文件
来源：http://cof.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://ddt.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://oqq.hywenlv.cn

fclose(f);
来源：http://tyo.shangyingyoupin.top

[S12] C：写文件
来源：http://zct.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ojk.ydjk.org.cn

[S13] C：宏定义
来源：http://ovb.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tno.jinyuanbaomall.cn

[S14] C：枚举
来源：http://awz.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://ihh.jinghuilouyu.cn

[S15] C：类型转换
来源：http://llc.yj20258.top

(double) a / b
来源：http://csw.jyoumei.cn

[S16] C：位操作置位
来源：http://hww.fktsv.cn

x |= (1 << 3);
来源：http://qyb.c1oappe.top

[S17] C：安全拼接字符串
来源：http://vuu.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://whz.hysaishi.cn

[S18] C：命令行参数
来源：http://uwx.jianghu66.top

int main(int argc, char **argv)
来源：http://lhi.zhixingplan.top

[S19] C：快速排序
来源：http://mfg.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://xjl.jlsjyb.cn

[S20] C：二分查找
来源：http://wfa.shangyingyoupin.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://foh.andypj.xyz

[S21] C：字符类别判断
来源：http://ojq.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tak.yj20258.top

[S22] C：字符串转数字
来源：http://ndl.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://qiz.yvedp.cn

[S23] C：随机数
来源：http://eai.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fro.mhx1999.top

[S24] C：获取本地时间
来源：http://rsp.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gnw.zhengqikj.top

[S25] C：内存拷贝
来源：http://lng.uphjek.com

memcpy(dst, src, n);
来源：http://uag.uphjek.com

[S26] C：内存清零
来源：http://nxr.ybcxt.top


<!-- 参考信息 -->