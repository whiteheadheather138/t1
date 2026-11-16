代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://drw.cqqwz.cn

[Q50] 批量更新
来源：http://gml.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wwm.hesvh.cn

[Q51] 用子查询更新
来源：http://pag.quarkkingdee.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://spp.daria6918.cn

[Q52] 删除指定行
来源：http://ueb.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://cso.yuanzhike.top

[Q53] 按条件删除
来源：http://tne.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oue.jinqigfzy.top

[Q54] 清空表
来源：http://ztp.hammf.cn

TRUNCATE TABLE logs;
来源：http://nyl.zhaomingkeji.xyz

[Q55] 排名（并列占位）
来源：http://sbq.yongpay.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://prr.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://avy.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sey.0kj1m.cn

[Q57] 行号
来源：http://hip.yonumen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kse.xuetiantiany.cn

[Q58] 累计求和
来源：http://xfl.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aay.gaohongyu789.top

[Q59] 分组内累计
来源：http://mqb.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kge.tanke756.top

[Q60] 取上一行 / 下一行
来源：http://ykq.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kzb.zhongyouzk.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lob.hysaishi.cn

[Q61] 移动平均
来源：http://czp.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wdr.guannengcc.top

[Q62] 分组占比
来源：http://ijk.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fjh.xinyue.icu

[Q63] 开启事务
来源：http://gsp.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://upq.fanxiaobao.xyz

[Q64] 提交事务
来源：http://zoj.quarkkingdee.top

COMMIT;
来源：http://lhw.guowangkeji.top

[Q65] 回滚事务
来源：http://tjq.daria6918.cn

ROLLBACK;
来源：http://gsp.jqgfzy.top

[Q66] 行锁查询
来源：http://vol.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vxk.wangdashe.top

[Q67] 设置隔离级别
来源：http://wno.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nal.yongpay.top

[Q68] 保存点
来源：http://vql.aizwys.cn

SAVEPOINT sp1;
来源：http://hdt.jianghu66.top

ROLLBACK TO sp1;
来源：http://rwp.dashuyun.cn

[Q69] 查看执行计划
来源：http://ifh.hywenlv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eox.sufxvd.cn

[Q70] 更新统计信息
来源：http://sge.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://cvb.hfpthk.cn

[Q71] 查看建表语句
来源：http://hzh.yj202588.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lfz.ehwqpu.com

[Q72] 查看索引
来源：http://ezp.andypj.xyz

SHOW INDEX FROM users;
来源：http://eel.cqqwz.cn

[Q73] 查看表状态
来源：http://phk.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://uuk.bbcook.cn

[Q74] 强制使用索引
来源：http://blf.bjfxy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kdr.yvedp.cn

[Q75] 日期格式化
来源：http://ugr.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aez.fehbvm.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yqy.gzhubu.top

[Q76] 按天统计
来源：http://xnd.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ekz.cqqwz.cn

[Q77] 时间加减
来源：http://ung.yfazqb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://goj.cheryme.top

[Q78] 当前时间
来源：http://cuv.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blf.hysaishi.cn

[Q79] 字符串拼接
来源：http://dth.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wnl.pycfn.com

[Q80] 字符串截取
来源：http://lxu.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mka.fehbvm.com

[Q81] 字符串替换
来源：http://gxr.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://are.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://fub.fehbvm.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hoy.gotoacloud.top

[Q83] 大小写转换
来源：http://avz.gzhubu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xej.hfpthk.cn

[Q84] 去除首尾空格
来源：http://nqs.ehwqpu.com

SELECT TRIM(name) FROM users;
来源：http://kqf.guowangkeji.top

[Q85] 数值取整
来源：http://eyi.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uok.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://txx.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lsa.hesvh.cn

[Q87] JSON 字段做条件
来源：http://nbp.316326.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://axm.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://ern.yj202588.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ioh.cucudq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aob.dashuyun.cn

[Q89] 判断表是否存在
来源：http://fsy.havefunace.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tiy.fktsv.cn

[Q90] 生成序号列
来源：http://tuj.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cqk.yj20258.top

================================================================================
来源：http://snf.bjfxy.top

R. Bash 专题
来源：http://kfj.ydzc1.top

================================================================================
来源：http://ccn.jinyuanbaomall.cn

[R01] shebang 与严格模式
来源：http://jvr.epnwcf.com

#!/usr/bin/env bash
来源：http://emr.gaohongyu789.top

set -euo pipefail
来源：http://qmy.cashguo.top

[R02] 变量赋值与使用
来源：http://ogs.9152youxi.cn

name="Tom"; echo "$name"
来源：http://mbs.redwolf501.top

[R03] 只读变量
来源：http://qno.shanyushiyangkeji.top

readonly PI=3.14
来源：http://zgb.zdbjq.cn

[R04] 位置参数
来源：http://fkp.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eau.tianlin.xyz

[R05] 参数默认值
来源：http://ely.zycfv.cn

name="${1:-default}"
来源：http://ugu.hcnkem.com

[R06] 判断命令是否存在
来源：http://byg.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tqc.sysykeji.top

[R07] if 判断文件
来源：http://fob.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://seo.kuanghao11.cn

[R08] 数值比较
来源：http://mri.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mnx.hywenlv.cn

[R09] 字符串比较
来源：http://lnk.gotoacloud.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xbx.9152youxi.cn

[R10] 正则匹配
来源：http://jwa.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wej.yongpay.top

[R11] case 多分支
来源：http://hwq.zdbjq.cn

case "$1" in
来源：http://wmy.chenjidiqi.icu

start) echo "启动" ;;
来源：http://zgl.nanxinkj.top

stop)  echo "停止" ;;
来源：http://cst.jiagoushi.top

*)     echo "未知命令" ;;
来源：http://jgi.jinyuanbaomall.cn

esac
来源：http://gxy.mhx1999.top

[R12] for 遍历文件
来源：http://iyo.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://jau.xuetiantiany.cn

[R13] for 计数循环
来源：http://ihb.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://wtc.wangdashe.top

[R14] C 风格 for
来源：http://qau.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ovs.hnqzz.top

[R15] while 逐行读文件
来源：http://cav.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xyk.hammf.cn

[R16] until 等待条件
来源：http://bmy.feifeiyinyue.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uic.nwbrower.top

[R17] 数组定义与取值
来源：http://pyc.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://dfz.ydjk.org.cn

[R18] 遍历数组
来源：http://rju.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qog.xuetiantiany.cn

[R19] 数组长度
来源：http://qnr.jlsjyb.cn

echo "${#arr[@]}"
来源：http://wca.tianlin.xyz

[R20] 关联数组（字典）
来源：http://cir.epnwcf.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pkz.tarul.cn

[R21] 字符串长度
来源：http://vdf.hnqzz.top

echo "${#s}"
来源：http://mjw.yj20258.top

[R22] 截取子串
来源：http://uhu.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://aqs.hongshengwenyu.top

[R23] 字符串替换
来源：http://jge.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xkk.316326.xyz

[R24] 大小写转换
来源：http://nsg.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mpn.xuanzx.com

[R25] 去后缀 / 去前缀
来源：http://xsu.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wyy.9152youxi.cn

[R26] 命令替换
来源：http://oai.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://bkk.xuanzx.com

[R27] 算术展开
来源：http://xka.hcnkem.com

echo $((1 + 2 * 3))
来源：http://mbu.cashguo.top

[R28] 浮点运算
来源：http://ezi.sjlbkw.cn

echo "scale=2; 10/3" | bc
来源：http://sxs.zycfv.cn

[R29] 定义函数
来源：http://bfs.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://app.hnqzz.top

[R30] 函数返回状态码
来源：http://urc.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://ntj.zhengqikj.top

[R31] 局部变量
来源：http://gyw.xuanzx.com

f() { local x=1; echo "$x"; }
来源：http://xho.fengsongda.top

[R32] 参数个数校验
来源：http://zrs.yangfankeji.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://org.sweek.top

[R33] 捕获错误并提示行号
来源：http://kfl.chenzaomai.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eyc.meibo888.top

[R34] 退出时清理
来源：http://lco.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qvh.sxryk.cn

[R35] 后台执行并等待
来源：http://vmw.yueranfly.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lde.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://pjr.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vac.ybcxt.top

[R37] 把输出赋给变量
来源：http://ebh.chenzaomai.com

files=$(ls -1)
来源：http://kpt.guowangkeji.top

[R38] 管道串联
来源：http://qrr.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://qwh.ivvv.top

[R39] 重定向标准输出与错误
来源：http://mmq.yueranfly.top

cmd > out.log 2>&1
来源：http://pyu.tanke756.top

[R40] 追加写日志
来源：http://ufi.aibaodan.cn

echo "log" >> out.log
来源：http://dui.shzxlz.cn

[R41] 丢弃输出
来源：http://mta.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://baq.jyoumei.cn

[R42] 输入重定向
来源：http://ywy.svipenyu.cn

wc -l < a.txt
来源：http://nmp.gotoacloud.top

[R43] 按名字查找文件
来源：http://wsr.gzhubu.top

find . -name "*.log" -type f
来源：http://cff.haohaochexian.top

[R44] 按修改时间查找
来源：http://qkr.cucudq.cn

find . -mtime -7 -type f
来源：http://jlm.svipenyu.cn

[R45] 批量删除
来源：http://zai.tanke756.top

find . -name "*.tmp" -delete
来源：http://wtr.bjfxy.top

[R46] 递归替换文件内容
来源：http://qta.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ghu.xylfe.cn

[R47] sed 单行替换
来源：http://zoz.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://csj.hcnkem.com

[R48] awk 取指定列
来源：http://ieb.hfpthk.cn

awk '{print $1, $3}' a.txt
来源：http://pte.chenjidiqi.icu

[R49] awk 带条件
来源：http://pql.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vcz.cucudq.cn

[R50] awk 求和
来源：http://gyd.tarul.cn

awk '{s += $2} END {print s}' a.txt
来源：http://awi.cheryme.top

[R51] 排序去重取前几
来源：http://ovs.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tla.ehwqpu.com

[R52] 统计行数
来源：http://wib.jinqigufen.top

wc -l a.txt
来源：http://vpe.pycfn.com

[R53] 查看文件头与实时尾
来源：http://kky.shanyushiyangtech.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ony.yanxiufei.cn

[R54] 比较两个文件
来源：http://tmt.zhengqikj.top

diff a.txt b.txt
来源：http://uro.pycfn.com

[R55] 压缩与解压
来源：http://zwg.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hoa.feifeiyinyue.top

[R56] 远程拷贝
来源：http://gzg.tian-w.cn

scp file user@host:/path/
来源：http://gmv.yj20258.top

[R57] 远程执行命令
来源：http://sny.sxryk.cn

ssh user@host 'uptime'
来源：http://wgy.dashuyun.cn

[R58] 下载文件
来源：http://vvn.yvedp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fli.bjfxy.top

[R59] 发 POST JSON
来源：http://brl.jqgufenzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mzo.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://lrc.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ced.cashguo.top

[R61] 磁盘占用
来源：http://zjp.9152youxi.cn

df -h;  du -sh *
来源：http://ngx.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://foe.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://sst.tarul.cn

[R63] 内存与进程
来源：http://txi.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://ahi.andypj.xyz

[R64] 结束进程
来源：http://aqj.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://lvl.jqgfzy.top

[R65] 查看端口占用
来源：http://wzi.hammf.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qow.gzhubu.top

[R66] 定时任务
来源：http://ghg.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://qbg.zhoulong.xyz

[R67] 生成随机十六进制串
来源：http://xtp.guannengcc.top

openssl rand -hex 16
来源：http://jie.yj20258888.top

[R68] 计算文件校验值
来源：http://uqf.chenlongwang.top

sha256sum a.txt;  md5sum a.txt
来源：http://yct.zdbjq.cn

[R69] 生成随机密码
来源：http://jrq.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://jms.jianghu66.top

[R70] 时间戳与互转
来源：http://mcm.hammf.cn

date +%s;  date -d @1700000000
来源：http://ijl.quarkkingdee.top

[R71] 日期格式化
来源：http://wzb.nanxuanxn.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xak.hammf.cn

[R72] 等待端口就绪
来源：http://npw.ydjk.org.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xbq.epnwcf.com

[R73] 分割大日志
来源：http://qek.hcnkem.com

split -l 1000 big.log part_
来源：http://bzu.sjlbkw.cn

[R74] 批量重命名
来源：http://bel.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fbj.yuanzhike.top

[R75] 导出环境变量
来源：http://xyk.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://upj.yfazqb.com

[R76] 使用临时文件
来源：http://axt.yueranfly.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sry.xinyue.icu

[R77] 读取用户输入
来源：http://wnk.sweek.top

read -rp "请输入: " ans
来源：http://vjz.wangshuangyany.cn

[R78] 交互式菜单
来源：http://pvz.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://dbs.sweek.top

[R79] 解析命令行选项
来源：http://mnk.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uaz.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://ppo.uphjek.com

time ./run.sh
来源：http://ojl.yj20258.top

================================================================================
来源：http://nli.cqqwz.cn

S. C / C++ 专题
来源：http://vmt.jlsjyb.cn

================================================================================
来源：http://rmi.vehdjk.com

[S01] C：Hello World
来源：http://uyg.sjlbkw.cn

#include <stdio.h>
来源：http://avm.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mgo.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://tbv.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://knj.iojbl.cn

[S03] C：读入整数
来源：http://nhk.hywenlv.cn

int x; scanf("%d", &x);
来源：http://sjm.guowangkeji.top

[S04] C：字符串复制
来源：http://hwv.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://swj.nwbrower.top

[S05] C：字符串长度
来源：http://gqn.fzhhl.top

strlen(s)
来源：http://zdi.yfazqb.com

[S06] C：字符串比较
来源：http://hje.hesvh.cn

strcmp(a, b) == 0
来源：http://mgn.guowangkeji.top

[S07] C：数组遍历求和
来源：http://mmo.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cuv.yj202588.top

[S08] C：动态内存分配与释放
来源：http://riy.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gso.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://hji.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bvv.zhoulong.xyz

[S10] C：指针与解引用
来源：http://jvf.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://pwn.xylfe.cn

[S11] C：逐行读文件
来源：http://nyl.tanke756.top

FILE *f = fopen("a.txt", "r");
来源：http://spc.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ldc.chenjidiqi.icu

fclose(f);
来源：http://kku.yongpay.top

[S12] C：写文件
来源：http://fgq.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://psv.zhaomingkeji.xyz

[S13] C：宏定义
来源：http://qvr.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mic.guannengcc.top

[S14] C：枚举
来源：http://rig.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://vda.jinqigfzy.top

[S15] C：类型转换
来源：http://dur.hywenlv.cn

(double) a / b
来源：http://aex.fengsongda.top

[S16] C：位操作置位
来源：http://xvl.andypj.xyz

x |= (1 << 3);
来源：http://dle.sweek.top

[S17] C：安全拼接字符串
来源：http://mwk.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xbg.jlsjyb.cn

[S18] C：命令行参数
来源：http://sxh.pycfn.com

int main(int argc, char **argv)
来源：http://mwg.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://ubu.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://qlw.zdbjq.cn

[S20] C：二分查找
来源：http://oak.hfpthk.cn


<!-- 参考信息 -->